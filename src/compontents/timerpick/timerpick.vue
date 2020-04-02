<template>
  <view>
    <view v-if="dialogVisible" class="timerpick_content animated fadeInUp">
      <view class="timerpick_cancel" @click="visible=false">取消</view>
      <view class="timerpick_sure" @click="suredaily()">确定</view>
      <picker-view
        indicator-style="height: 50px;line-height:50px" style="width: 100%; height: 300px;"
        :value="value"
        @change="bindChange"
      >
        <picker-view-column>
          <view class="item" v-for="(item,index) in years" :key="index">{{item}}年</view>
        </picker-view-column>
        <picker-view-column>
          <view class="item" v-for="(item,index) in months" :key="index">{{item}}月</view>
        </picker-view-column>
        <picker-view-column>
          <view class="item" v-for="(item,index) in days" :key="index">{{item}}日</view>
        </picker-view-column>
      </picker-view>
    </view>
  </view>
</template>

<script>
  export default {
    props: {
      dialogVisible: {
        type: Boolean,
        default: false
      }
    },
    data: function() {
      const date = new Date();
      const years = [];
      const year = date.getFullYear();
      const months = [];
      const month = date.getMonth() + 1;
      const days = [];
      const day = date.getDate();
      for (let i = 1980; i <= date.getFullYear(); i++) {
        years.push(i);
      }
      for (let i = 1; i <= 12; i++) {
        months.push(i);
      }
      for (let i = 1; i <= 31; i++) {
        days.push(i);
      }
      return {
        visible_picket: true,
        title: "picker-view",
        years,
        year,
        months,
        month,
        days,
        day,
        value: [9999, month - 1, day - 1],
      };
    },
    onLoad() {
      console.log('this.years++', this.years)
      console.log("111", uni.getSystemInfoSync());
    },
    methods: {
      bindChange: function(e) {
        const val = e.detail.value;
        this.year = this.years[val[0]];
        this.month = this.months[val[1]];
        this.day = this.days[val[2]];
      },
      suredaily() {
        this.visible_picket = false
      }
    }
  };
</script>
<style lang="scss">
  .timerpick_content {
    position: absolute;
    width: 100%;
    bottom: 0;
    padding-top: 60rpx;
    .item,view {
      line-height: 50px;
    }
    .timerpick_cancel {
      color: #ccc;
      position: absolute;
      left: 10rpx;
      top: 15rpx;
      font-size: 30rpx;
      line-height: 1;
    }
    .timerpick_sure {
      color: rgb(33, 224, 65);
      position: absolute;
      right: 10rpx;
      top: 15rpx;
      font-size: 30rpx;
      line-height: 1;
    }
  }
</style>
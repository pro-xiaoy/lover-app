
<template>
  <div class="home_bg">
    <div class="home_dayils">
      <div class="home_dayils-item">
        <img src="@/static/archer1.png" alt />
      </div>
      <div class="home_dayils-item-text">
        在一起已经
        <p>
          <span class="home_dayils-item-text_b">385</span>天
        </p>
      </div>
      <div class="home_dayils-item">
        <img src="@/static/sabar1.png" alt />
      </div>
    </div>
    <div class="home_foot_items">
      <div class="home_foot_item">
        <img class="home_foot_item-img" src="@/static/rili.png" alt="">
        <p class="home_foot_item-title">纪念日</p>
        <p class="home_foot_item-daily">估计30天</p>
      </div>
      <div class="home_foot_item">
        <img class="home_foot_item-img" src="@/static/jinianri.png" alt="">
        <p class="home_foot_item-title">纪念日</p>
        <p class="home_foot_item-daily">估计30天</p>
        <!-- 私密日记 -->
      </div>
      <div class="home_foot_item">
        <img class="home_foot_item-img" src="@/static/yunzhushou.png" alt="">
        <p class="home_foot_item-title">纪念日</p>
        <p class="home_foot_item-daily">估计30天</p>
        <!-- 姨妈助手 -->
      </div>
    </div>
  </div>
</template> 

<script>
import { mapState } from "vuex";

export default {
  data() {
    return {};
  },
  onLaunch() {
    console.log("2222");
  },
  mounted() {
    console.log(this.UserInfo);
  },
  computed: mapState({
    UserInfo: state => state.UserInfo
  }),
  methods: {
    hreflink() {
      console.log("1");
      uni.navigateTo({
        url: "/compontents/demoone/demoone"
      });
    }
  }
};
</script>

<style lang="scss">
.home_bg {
  width: 100%;
  height: 100vh;
  background-size: contain;
  background-image: url("https://hbimg.huabanimg.com/4f04e12ef33495b8f8080a300e64bd30c73ed88fd297c-gmKHQW_fw658");
  display: flex;
  .home_bound-btn {
    width: 278rpx;
    margin: 40rpx auto 0;
    height: 166rpx;

    text-align: center;
    color: #fff;
    background: rgba($color: #000000, $alpha: 0.4);
    line-height: 166rpx;
    border-radius: 10rpx;
  }
  .home_dayils {
    width: 514rpx;
    height: 200rpx;
    background: rgba($color: #000000, $alpha: 0.4);
    position: relative;
    margin-top: 110rpx;
    border-radius: 0 80rpx 80rpx 0;
    display: flex;
    // flex-direction: column;
    justify-content: space-around;
    align-items: center;
  }
  .home_dayils-item {
    width: 102rpx;
    height: 102rpx;
    border-radius: 50%;
    box-sizing: border-box;
    float: left;
    overflow: hidden;
    border: 1rpx solid #479eed;
    img {
      width: 100%;
    }
  }
  .home_dayils-item-text {
    text-align: center;
    color: black;
    font-size: 30rpx;
    line-height: 60rpx;
    .home_dayils-item-text_b {
      font-size: 40rpx;
      font-weight: bold;
    }
  }
  .home_foot_items {
    position: absolute;
    bottom: 10rpx;
    width: 750rpx;
    display: flex;
    justify-content: space-around;
    .home_foot_item {
      width: 220rpx;
      height: 220rpx;
      border-radius: 50%;
      background: #fff;
      text-align: center;
      &:nth-child(2) {
        margin-top: -40rpx;
      }
    }
    .home_foot_item-img {
      width: 72rpx;
      height: 72rpx;
      padding-top: 30rpx;
    }
    .home_foot_item-title {
      text-align: center;
    }
    .home_foot_item-daily {
      text-align: center;
      color: #e8e8e8;
    }
  }
}
</style>

<style >
</style>
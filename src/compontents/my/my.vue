
<template>
  <view class="my">
    <view class="my-head">
      <view class="head_avlar-info">
        <view class="head-avlar"></view>
        <view class="head-avlar"></view>
        <view class="head-avlar"></view>
      </view>
      <view class="head_nickname-info">
        <view class="head_nickname">二狗子</view>
        <view class="head_nickname">小仙女</view>
      </view>  
      <view class="head_timer-info">
        <view class="head_timer">二狗子</view>
        <view class="head_timer">小仙女</view>
      </view>  
    </view>
  </view>
</template> 

<script>
export default {};
</script>
<style lang="scss">
.my {
  .my-head {
    width: 754rpx;
    height: 448rpx;
    background-color: #eb535f;
    margin: 50rpx auto 0;
    .head_avlar-info {
      width: 500rpx;
      height: 110rpx;
      background: rgba(250, 250, 250, 0.5);
      display: flex;
      justify-content: space-between;
    }
    .head-avlar {
      width: 124rpx;
      height: 124rpx;
      background-color: #ffffff;
      border-radius: 50%;
    }
    .head_nickname-info {
      width: 500rpx;
      margin: 20rpx auto 0;
      display: flex;
      justify-content: space-between;
    }
    .head_nickname {
      color: #fff;
    }
    .head_timer-info {
       width: 540rpx;
       margin: 20rpx auto;
    }
  }
}
</style>
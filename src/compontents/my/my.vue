
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
        <view class="head_timer">
          相爱于
          <p>2019年12月17日</p>
        </view>
        <view class="head_timer">
          记录时刻
          <p>4个</p>
        </view>
      </view>
    </view>
    <!-- 752 454 -->
    <view class="my-lists">
      <view class="my-list">
        <img class="my-list-icon" src="@/static/pencil.png" alt />
        <span>情侣资料</span>
        <img class="my-list-crow" src="@/static/right-arrow.png" alt />
      </view>
      <view class="my-list">
        <img class="my-list-icon" src="@/static/video.png" alt />
        <span>恋爱video</span>
        <img class="my-list-crow" src="@/static/right-arrow.png" alt />
      </view>
      <view class="my-list">
        <img class="my-list-icon" src="@/static/wenti.png" alt />
        <span>常见问题</span>
        <img class="my-list-crow" src="@/static/right-arrow.png" alt />
      </view>
      <view class="my-list">
        <img class="my-list-icon" src="@/static/kefu.png" alt />
        <span>联系客服</span>
        <img class="my-list-crow" src="@/static/right-arrow.png" alt />
      </view>
    </view>
    <view class="my-footer">我有个愿望，希望等我们白发时， 能细数有你在的恋爱时光</view>
  </view>
</template> 

<script>
export default {};
</script>
<style lang="scss">
.my {
  overflow: hidden;
  .my-head {
    width: 680rpx;
    height: 448rpx;
    background-color: #eb535f;
    margin: 50rpx auto 0;
    border-radius: 60rpx;
    padding-top: 1rpx;
    .head_avlar-info {
      width: 500rpx;
      height: 124rpx;
      margin: 36rpx auto 0;
      background: rgba(250, 250, 250, 0.5);
      display: flex;
      justify-content: space-between;
      border-radius: 62rpx;
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
      margin: 80rpx auto;
      display: flex;
      justify-content: space-between;
      color: #fff;
    }
    .head_timer {
      text-align: center;
    }
  }
  .my-lists {
    width: 656rpx;
    margin: 70rpx auto 0;
  }
  .my-list {
    width: 100%;
    height: 114rpx;
    box-sizing: border-box;
    border-bottom: 1rpx solid #ccc;
    position: relative;
    padding-left: 130rpx;
    line-height: 114rpx;
    color: #222;
  }
  .my-list-icon {
    width: 50rpx;
    height: 50rpx;
    position: absolute;
    top: 32rpx;
    left: 2rpx;
  }
  .my-list-crow {
    position: absolute;
    width: 40rpx;
    height: 40rpx;
    right: 20rpx;
    top: 37rpx;
  }
  .my-footer {
    position: absolute;
    text-align: center;
    bottom: 20rpx;
    width: 500rpx;
    left: 125rpx;
  }
}
</style>
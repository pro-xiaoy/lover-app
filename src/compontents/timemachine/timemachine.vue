<template>
  <div class="time">
    <div class="time-head">
      <div class="time-head-headers clearfix">
        <div class="time-head-header"></div>
        <div class="time-head-header"></div>
      </div>
      <div class="time-head-conunts">
        <p>共记录</p>
        <p>4个时刻</p>
      </div>
    </div>
    <div class="time-log">
      <div class="time-log_left">2019</div>
      <div class="time-log_right"></div>
    </div>
    <div class="time-content">

    </div>
    <div class="time_add">+</div>
  </div>
</template>
<script>

</script>
<style lang="scss">
.time {
  .time_add {
    position: fixed;
    bottom: 100rpx;
    right: 40rpx;
    width: 100rpx;
    border-radius: 50%;
    background: #eb535f;
    color: #fff;
    font-size: 60rpx;
    font-weight: bold;
    text-align: center;
    line-height: 100rpx;
  }
  .time-head {
    width: 100%;
    height: 460rpx;
    position: relative;
     background-color: #ccc;
  }
  .time-head-headers {
    position: absolute;
    left: 34rpx;
    bottom: 34rpx;
  }
  .time-head-header {
    float: left;
    height: 100rpx;
    width: 100rpx;
    border-radius: 50%;
    background-color: #fff;
    &:nth-child(2) {
      margin-left: -40rpx;
    }
  }
  .time-head-conunts {
     position: absolute;
    right: 34rpx;
    bottom: 34rpx;
    p{
      color: #e0e0e0;
      text-shadow:5px 2px 6px #000;
      line-height: 30rpx;
    }
  }
  .time-log {
    width: 100%;
    height: 96rpx;
    display: flex;
    padding: 30rpx 40rpx;
    line-height: 1;
    justify-content: space-between;
    box-sizing: border-box;
    box-shadow: 5px 1px 6px #000;;
  }
  .time-content {
    background: #ccc;
    width: 100%;
    height: 100vh;
  }
}
</style>
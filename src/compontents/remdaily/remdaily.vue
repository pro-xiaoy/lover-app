<template>
  <view>
    <view class="remdaily_btn">CNM</view>
    <time-picket :visible="dialogVisible"></time-picket>
  </view>
</template>
<script>
import timePicket from '../timerpick/timerpick'
export default {
  data() {
    return {
      dialogVisible: false
    }
  },
  components: {
    'timePicket': timePicket
  }
}
</script>
<style lang="scss">

</style>
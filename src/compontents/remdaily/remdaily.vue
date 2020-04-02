<template>
  <view>
    <view class="remdaily_btn" @click="showtime">CNM</view>
    <time-picket :visible="dialogVisible" @timeClose="timeClose"></time-picket>
  </view>
</template>
<script>
import timePicket from "../timerpick/timerpick";
export default {
  data() {
    return {
      dialogVisible: true
    };
  },
  components: {
    timePicket: timePicket
  },
  methods: {
    showtime() {
      this.dialogVisible = true;
    },
    timeClose(val) {
      this.dialogVisible = val;
    }
  }
};
</script>
<style lang="scss">
</style>
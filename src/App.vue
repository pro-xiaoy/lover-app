<script>
export default {
  onLaunch: function() {
  //  当uni-app 初始化完成时触发（全局只触发一次）
    const userInfo = uni.getStorageSync("userInfo");
    if (userInfo) {
      this.$store.commit("SET_USERINFO", userInfo);
    }
    this.getInfo();

  },
  onShow: function() {},
  onHide: function() {},
  methods: {
    getInfo() {
      this.$store.dispatch('wxlogin')
    }
  }
};
</script>

<style>
@import './common/style/common.css';
@import './common/style/uni.css';
@import './common/style/animate.min.css'
/*每个页面公共css */
</style>

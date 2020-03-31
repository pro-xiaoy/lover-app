<script>
export default {
  onLaunch: function() {
    uni.getUserInfo({
        success: (res) => {
          var userInfo = res.userInfo
          if (userInfo) this.$store.commit('SET_USERINFO', userInfo)
        
          // state.userInfo = Object.assign({}, state.userInfo, userInfo)
          // var nickName = userInfo.nickName
          // var avatarUrl = userInfo.avatarUrl
          // var gender = userInfo.gender //性别 0：未知、1：男、2：女
          // var province = userInfo.province
          // var city = userInfo.city
          // var country = userInfo.country
        }
      })
  },
  onShow: function() {
  },
  onHide: function() {
  }
};
</script>

<style>
/*每个页面公共css */
</style>

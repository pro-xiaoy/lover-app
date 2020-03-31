
<template>
  <div class="">
    home
    {{UserInfo}}
  </div>
</template> 

<script>
	import { mapState } from 'vuex'

export default {
  data() {
    return {

    }
  },
  computed: {
			...mapState([
				'UserInfo'
			])
		}
}
</script>
<style lang="sass">

</style>
<template>
	<view>
		<Home />
	</view>
</template>
<script>
	import Home from './pages/home/index.vue'
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		},
		components:{
			Home
		}
	}
</script>

<style>
	/*每个页面公共css */
</style>

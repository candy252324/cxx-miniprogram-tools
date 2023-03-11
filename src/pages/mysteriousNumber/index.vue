<template>
	<view class="content">
    神秘数字
	</view>
</template>

<script lang="ts">
  import Vue from 'vue';
	export default Vue.extend({
		data() {
			return {
				toolsList:[{text:"图片加 水印"}]
			}
		},
		created(){console.log("created")},
		onLoad() {
			console.log("onload")

		},
		methods: {

		}
	});
</script>

<style>
	/* .content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin: 200rpx auto 50rpx auto;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	} */
</style>

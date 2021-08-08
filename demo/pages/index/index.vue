<template>
	<view class="content">
		<aki-particles :particlestyle="particlestyle"></aki-particles>
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
	</view>
</template>

<script>
	import akiparticles from '../../uni_modules/aki-particles/components/aki-particles/aki-particles.vue'//导入组件
	export default {
		components:{"aki-particles":akiparticles},//组件声明
		data() {
			return {
				title: 'Hello',
				particlestyle:{
					"style":"akira",
					"zindex":1,
					"bgcolor":"#000022"
				},
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.content {
		display: flex;
		flex-direction: column;
		// align-items: center;
		 justify-content: center;
	}

	.logo {
		z-index: 2;
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		z-index: 2;
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>

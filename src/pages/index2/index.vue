<template>
	<view class="content">
		<view class="rpx">rpx</view>
		<view class="vw">vw</view>
		<view class="sass">sass</view>
</view>
</template>

<script>

export default {

}
</script>

<style lang="scss">
.rpx {
	width: 750rpx;
	height: 100px;
	background-color: cyan;
}

.vw {
	width: 50vw;
	height: 50vw;
	background-color: tan;
}

.content {
	.sass {
		background-color: $uni-color-title;
		color: $uni-color-error
	}
}
</style>

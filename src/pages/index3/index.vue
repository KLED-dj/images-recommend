<template>
	<view class="content">
		<view>{{ msg }}</view>
		<view>{{ price }}</view>
		<view>{{ isRich }}</view>
		<view>{{ person.name }}</view>
		<view>{{ person.skill }}</view>
		<!-- 在标签上 通过属性的方式使用数据-->
		<view v-bind:data-color="color">color</view>

		<view>============================</view>
		<view v-for="( item ) in list" :key="item.id">
			{{ item.text }}--{{ item.id }}
		</view>
</view>
</template>
<script>


export default {
	data() {
		return {
			msg: "nihao",
			price: 1000,
			isRich: false,
			person: {
				name: "悟空",
				skill: "大闹天宫"
			},
			color: "red",
			list: [
				{
					id: 0,
					text: "苹果"
				},
				{
					id: 1,
					text: "香蕉"
				},
				{
					id: 2,
					text: "梨"
				}
			]
		}
	}
}
</script>

<style lang="scss"></style>

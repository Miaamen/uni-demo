<template>
	<view>
		<tabs class="border-bottom">
            <tab-item v-for="tab, index in tabs" :key="index" :name="tab.name" :label="tab.label" />
        </tabs>
		<comment-list :comment-param="commentParam"></comment-list>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				commentParam: {
					snid: 'BD20200202',
					//  snid: 'test_123',
					path: '/pages/comment/index?snid=BD20200202',
					title: '测试文章标题',
					content: '测试文章内容'
				},
				tabs: [{
					name: '一',
					label: '标签一'
				}, {
					name: '二',
					label: '标签二'
				}, {
					name: '三',
					label: '标签三'
				}]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
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
	}
</style>

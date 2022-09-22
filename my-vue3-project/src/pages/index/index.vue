<template>
    <view class="content">
        <comment-list class="list"
            is-folded="true"
            :comment-param="commentParam"
        ></comment-list>
    </view>
</template>

<script>
    export default {
        setup() {
            return {
                title: 'hello',
                commentParam: {
                    snid: 'BD20200202',
                    //  snid: 'test_123',
                    path: '/pages/comment/index?snid=BD20200202',
                    title: '测试文章标题',
                    content: '测试文章内容'
                }
            }
        }
    }
</script>

<style>
</style>

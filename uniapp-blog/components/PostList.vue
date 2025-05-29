<template>
  <view>
    <block v-for="post in posts" :key="post.id">
      <navigator :url="'/pages/posts/posts?id=' + post.id">
        <view class="post-item">
          <text class="post-title">{{ post.title }}</text>
        </view>
      </navigator>
    </block>
  </view>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        { id: 1, title: 'Hello World' },
        { id: 2, title: 'First Post' }
      ]
    }
  }
}
</script>

<style>
.post-item {
  padding: 20rpx;
  border-bottom: 1px solid #e5e5e5;
}
.post-title {
  font-size: 32rpx;
}
</style>

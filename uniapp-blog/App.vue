<template>
  <view class="container">
    <Header />
    <router-view />
  </view>
</template>

<script>
import Header from './components/Header.vue'
export default {
  components: { Header }
}
</script>

<style>
.container {
  padding: 20rpx;
}
</style>

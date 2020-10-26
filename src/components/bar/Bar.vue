<template>
  <view class="main">
    <view :style="{backgroundColor: color}" class="left"> </view>

    <text class="title">{{ title }}</text>

    <view :style="{backgroundColor: color}" class="right">更多> </view>
  </view>
</template>

<script>
export default {
  props: ["title", "color"],
};
</script>

<style scoped>
.main {
  display: flex;
  justify-content: space-between;
  height: 53rpx;
  padding-left: 2%;
  padding-right: 4%;
  margin: 30rpx 0;
}

.left {
  width: 14rpx;
  height: 100%;
}

.title {
  font-size: 34rpx;
  margin-top: 6rpx;
  margin-right: 62%;
}

.right {
  margin-top: 20rpx;
  width: 65rpx;
  height: 34rpx;
  border-radius: 20rpx;
  font-size: 16rpx;
  line-height: 34rpx;
  text-align: center;
  color: #ffffff;
}
</style>

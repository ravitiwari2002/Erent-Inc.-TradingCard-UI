<template>
  <view class="status-bar">
    <text class="time">9:41</text>
    <view class="status-icons">
      <text class="signal">●●●●</text>
      <text class="wifi">📶</text>
      <text class="battery">🔋</text>
    </view>
  </view>
</template>

<style scoped lang="scss">
.status-bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20rpx 40rpx;
  padding-top: 80rpx;
  z-index: 10;
  .time { color: #fff; font-size: 32rpx; font-weight: 600; }
  .status-icons {
    display: flex; gap: 10rpx; align-items: center;
    .signal, .wifi, .battery {
      color: #fff; font-size: 32rpx;
    }
  }
}
</style>

<template>
  <view class="container">
    <StatusBar />
    <view class="main-content">
      <TotalAssets />
      <MyCollections @browse="onBrowseClick" @claim="onClaimClick" />
    </view>
    <BottomNav />
  </view>
</template>


<script>
import StatusBar from '@/components/StatusBar.vue'
import TotalAssets from '@/components/TotalAssets.vue'
import MyCollections from '@/components/MyCollections.vue'
import BottomNav from '@/components/BottomNav.vue'

export default {
  name: 'MyCollectionPage',
  components: {
    StatusBar,
    TotalAssets,
    MyCollections,
    BottomNav
  }
}
</script>

<style lang="scss">
.container {
  width: 100%;
  min-height: 100vh;
  background: linear-gradient(270deg, #2D0A3D 0%, #14081D 100%);
  display: flex;
  flex-direction: column;
  position: relative;
  overflow-y: auto;
  box-sizing: border-box;
}


.main-content {
  flex: 1;
  padding: 4vh 6vw 0;
  max-width: 750rpx;
  margin: 0 auto;
  width: 100%;
  box-sizing: border-box;
  padding-bottom: 120rpx;
}
</style>

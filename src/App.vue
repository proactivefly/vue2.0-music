<template>
  <div id="app" @touchmove.prevent>
    <!-- header组件 -->
    <m-header></m-header>
    <!-- 顶部导航 -->
    <tab></tab>
    <!-- keep-alive保存之前页面状态 -->
    <keep-alive>
      <!-- 试图渲染层 -->
      <router-view></router-view>
    </keep-alive>
    <!-- 个人中心 -->
    <player></player>
  </div>
</template>

<script type="text/ecmascript-6">
  import MHeader from 'components/m-header/m-header'
  import Player from 'components/player/player'
  import Tab from 'components/tab/tab'

  export default {
    components: {
      MHeader,
      Tab,
      Player
    }
  }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
</style>
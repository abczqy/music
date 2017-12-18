<template>
  <div id="app">
    <m-header></m-header>
    <tab></tab>
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
    <player></player>
  </div>
</template>

<script type="text/ecmascript-6">
  import MHeader from '@/components/m-header/m-header'
  import Tab from '@/components/tab/tab'
  import Recommend from '@/components/recommend/recommend'
  import Player from 'components/player/player'

  export default {
    components: {
      MHeader,
      Tab,
      Recommend,
      Player
    }
  }
</script>

<style scoped rel="stylesheet/stylus" lang="stylus">
  @import "common/stylus/variable"

  #app
    color: $color-theme
</style>

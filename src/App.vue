<template>
    <div id="app">
      <router-view></router-view>
      <FootGuide v-show="$route.meta.showFooter"/>
    </div>
</template>

<script>
    import FootGuide from './components/FooterGuide/FooterGuide.vue'
    export default {
      //映射成标签
      components: {
        FootGuide
      }
    }
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .app
    width 100%
    height 100%
    background #f5f5f5
</style>

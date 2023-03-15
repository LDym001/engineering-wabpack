<template>
  <div id="app">
    <header>hi...</header>
    <test-view></test-view>
  </div>
</template>

<script>
import TestView from '@/views/test-view'
export default {
  name: 'App',
  components: { TestView },
}
</script>

<style lang="less" scoped>
.app {
  header {
    text-align: center;
    color: antiquewhite;
  }
}
</style>

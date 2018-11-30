<template>
  <div id="app">
    <page-header></page-header>
    <router-view></router-view>
  </div>
</template>

<script>
import pageHeader from '@/components/page-header/page-header'
export default {
  name: 'App',
  conponents: {
    pageHeader
  }
}
</script>

<style>
@import './assets/less/base.less';
</style>

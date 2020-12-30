<template>
  <div id="app">
    <router-view></router-view>
    <main-tab-ber/>
  </div>
</template>

<script>
import MainTabBer from './components/MainTabBer/MainTabBer'
export default {
  name: 'App',
  components: {
    MainTabBer
  }
}
</script>

<style>
/* 在style中引入东西的时候就用@import */
@import "./assets/css/base.css"; 



</style>

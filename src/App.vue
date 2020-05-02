<template>
  <div id="app">
    <Overview/>
  </div>
</template>

<script>
import Overview from './views/Overview.vue'
export default {
  name: 'App',
  components: {
    Overview
  }
}
</script>

<style>
html {
    box-sizing: border-box;
 }
 *, *::before, *::after {
    box-sizing: inherit;
 }

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<template>
  <div id="app">
    <UkulelePage />
  </div>
</template>

<script>
import UkulelePage from './components/pages/UkulelePage.vue'

export default {
  name: 'App',
  components: {
    UkulelePage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e60;
  margin-top: 60px;
}
</style>

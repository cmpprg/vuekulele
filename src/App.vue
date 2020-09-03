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
  color: #2c3e60;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

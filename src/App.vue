<template>
  <div id="app">
    <Ukulele/>
  </div>
</template>

<script>
import Ukulele from './components/pages/Ukulele.vue'

export default {
  name: 'App',
  components: {
    Ukulele
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

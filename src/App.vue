<template>
  <div id="app">
    <button v-on:click='isLanding = true'>Home</button>
    <button v-on:click='isLanding = false'>Ukulele</button>
    <UkulelePage v-if='!isLanding'/>
    <LandingPage v-if='isLanding'/>
  </div>
</template>

<script>
import UkulelePage from './components/pages/UkulelePage.vue'
import LandingPage from './components/pages/LandingPage.vue'

export default {
  name: 'App',
  components: {
    UkulelePage,
    LandingPage
  },
  data() {
    return {
      isLanding: false
    }
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

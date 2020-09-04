<template>
  <div id="app">
    <Navbar :toggleIsLanding='toggleIsLanding'/>

    <UkulelePage v-if='!isLanding'/>
    <LandingPage v-if='isLanding'/>

    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar'
import UkulelePage from './components/pages/UkulelePage.vue'
import LandingPage from './components/pages/LandingPage.vue'
import Footer from './components/Footer'
export default {
  name: 'App',
  components: {
    Navbar,
    UkulelePage,
    LandingPage,
    Footer
  },
  data() {
    return {
      isLanding: true
    }
  },
  methods: {
    toggleIsLanding: function(boolean) {
      this.isLanding = boolean
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
  padding-bottom: 5%;

  width: 100%;
  height: 100%;
}
</style>

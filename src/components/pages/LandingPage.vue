<template>
  <div class="landing">
    <Header title='Aloha!'/>
    <Card
      alignment='left'
      title="About This Project"
      text="Welcome to Vuekulele! This app is an online manual music maker modeled after the one and only Ukulele.
            This project was initiated by the Vue.js Hackathon, hosted by Mintbean.
            We were given approximately 48 hours to contruct this application using only front-end technologies including Vue.js "
    />
    <Card
      alignment='right'
      title="How To Use This App"
      text="To use this app"
    />
    <Card
      alignment='left'
      title="Technologies Used / Learned"
      text="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
    />
    <div class="last-element">
      <Card
      alignment='right'
      title="Nice To Meet You!"
      text="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
      />
    </div>
  </div>
</template>

<script>
  import Header from '../Header.vue'
  import Card from '../Card.vue'

  export default {
    name: "LandingPage",
    components: {
      Header,
      Card
    }
  }
</script>

<style scoped>
  hr {
    display: block;
  }
  .landing {
    padding-bottom: 10%;
  }

  .last-element {
    margin-bottom: 100px;
  }
</style>

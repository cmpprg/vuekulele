<template>
  <div class="landing">
    <Header title='Aloha!'/>
    <Card
      alignment='left'
      title="About This Project"
      text="Welcome to Vuekulele! This app is an online manual music maker modeled after the one and only Ukulele.
            This project was initiated by the Vue.js Hackathon, hosted by Mintbean.
            We were given approximately 48 hours to construct this application using Vue.js and other Front-End Technologies. "
    />
    <Card
      alignment='right'
      title="How To Use This App"
      text="To use this app first navigate to the Instrument Page. You can find the navigation at the top of this page. On the instrument page you will find
            a fret board modeled after a Ukulele. You will see labels telling you the note and octave of each fretted position along the neck of the Ukulele.
            If you click on any of these notes, that frequency will play for you. Please note that on the far left there is a column called 'OPEN', when you click
            these notes it's as if your plucking a string without holding down any strings."
    />
    <Card
      alignment='left'
      title="Technologies Used / Learned"
      text="Vue.js and Tone.js"
    />
    <div class="last-element">
      <Card
      alignment='right'
      title="Nice To Meet You!"
      text="Hey there! My name is Ryan Camp. I am a Software Engineer with a passion for learning and implementing new technologies.
            I have varying interests ranging from web design to robotics. I have always wanted to build my own AI personal assistant... Maybe someday...
            If you have need of a quick learning individual who loves working with others, takes developer empathy seriously and gets the job done please reach out.
            Even if you don't have need and just want to meet and chat about technology.
            You can contact me utilizing one of the methods located in the footer. I hope you have a greate day!"
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
      Card,
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

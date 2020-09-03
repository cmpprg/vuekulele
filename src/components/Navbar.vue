<template>
  <div class="container">
    <div class='nav-button home' @click='toggleIsLanding(true)'>Home</div> |
    <div class='nav-button instrument' @click='toggleIsLanding(false)'>Ukulele</div>
  </div>
</template>

<script>
  export default {
    name: "Navbar",
    props: {
      toggleIsLanding: Function
    }
  }
</script>

<style scoped>
  .container {
    background-color: gray;
    color: white;
    border-radius: 0px 0px 20% 20%;
    padding-left: 20%;
  }

  .nav-button {
    display: inline-block;
    padding: 15px;
    font-size: 20px;
  }

  .nav-button:hover {
    cursor: pointer;
    background-color: #281b0d;
  }

  .home:hover {
    border-left: 0.5px solid #ffffff;
    border-bottom: 0.5px solid #ffffff;
  }

  .instrument:hover {
    border-right: 0.5px solid #ffffff;
    border-bottom: 0.5px solid #ffffff;
  }

</style>

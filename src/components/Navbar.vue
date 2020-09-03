<template>
  <div class="container">
    <div class='nav-button' @click='toggleIsLanding(true)'>Home</div> |
    <div class='nav-button' @click='toggleIsLanding(false)'>Ukulele</div>
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
    border-radius: 0px 0px 20px 20px;
  }

  .nav-button {
    display: inline-block;
    margin: 20px;
    font-size: 20pxpx;
  }

  .nav-button:hover {
    cursor: pointer;
  }
</style>

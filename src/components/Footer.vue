<template>
  <div class="footer">
    <div class="labels">
      <p>Vuekulele | CampPRG</p>
    </div>
    <div class="links">
      <p>campryan@comcast.net</p>
      <a href="https://github.com/cmpprg"><img src="../assets/GitHub-Mark-32px.png" alt="Ryan Camp's Github Profile"></a>
      <a href="https://www.linkedin.com/in/campprg/"><img src="../assets/LI-In-Bug.png" alt="Ryan Camp's LinkedIn Profile"></a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Footer"
  }
</script>

<style scoped>
  .footer {
    height: 8%;
    position: fixed;
    bottom: 0;
    width: 100%;
    border-radius: 20% 20% 0 0;
    background-color: gray;
    color: white;
  }

  .labels {
    display: inline-block;
    margin-left: 20%;
  }

  .links {
    display: inline-block;
    float: right;
    margin-right: 15%;
  }

  p, a {
    display: inline-block;
    font-size: 20px;
    color: white;
    text-decoration: none;
    padding: 0px 15px;
  }

  img {
    width: 25px;
    height: auto;
  }

</style>

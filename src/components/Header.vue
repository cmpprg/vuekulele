<template>
  <div class="container">
    <p>{{title}}</p>
  </div>
</template>

<script>
  export default {
    name: "Header",
    props: {
      title: String
    }
  }
</script>

<style scoped>

  .container {
    margin:auto;
    margin-bottom: 10%;
    width: 20%;
    text-align: center;
    font-size: 40px;
    text-decoration: underline;

  }
</style>

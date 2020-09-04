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
    width: 20%;
    text-align: center;
    text-decoration: underline;
    font-size: 40px;
    font-weight: 700;
    color: gray;
    -webkit-text-stroke: 1px white;
  }
</style>

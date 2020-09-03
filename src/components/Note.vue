<template>
  <div class="note">
    <p>{{keyOf}}</p>
  </div>
</template>

<script>
  export default {
    name: "Note",
    props: {
      keyOf: String
    }
  }
</script>

<style scoped>
  .note {
    border: 2px solid black;
    display: inline-block;
    float: left;
    width: 50px;
    text-align: center;
  }
</style>

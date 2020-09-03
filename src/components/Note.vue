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
    boder: 2px solid black;
  }
</style>

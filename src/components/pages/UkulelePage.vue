<template>
  <div>
    <div class="title">
      <p>This is the Ukulele Page</p>
    </div>

    <div class="neck">
      <Neck />
    </div>
  </div>
</template>

<script>
  import Neck from '../Neck.vue'

  export default {
    name: "UkulelePage",
    components: {
      Neck
    }
  }
</script>

<style scoped>
  .title {
    padding-bottom: 15%;
    text-align: center;
  }
</style>

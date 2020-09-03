<template>
  <div>
    <div class="title">
      <p>Ukulele Page</p>
    </div>

    <div class="instrument">
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
  * {
  }
  .title {
    padding-top: 30px;
    padding-bottom: 15%;
    text-align: center;
    font-size: 20px;
  }
</style>

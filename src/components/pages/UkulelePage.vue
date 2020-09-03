<template>
  <div class="app">
    <Header title='Ukulele'/>
    <div class="instrument">
      <Neck />
    </div>
  </div>
</template>

<script>
  import Header from '../Header'
  import Neck from '../Neck.vue'

  export default {
    name: "UkulelePage",
    components: {
      Header,
      Neck
    }
  }
</script>

<style scoped>

  .title {
    padding-top: 30px;
    padding-bottom: 15%;
    text-align: center;
    font-size: 20px;
  }
</style>

<template>
  <div class="string">
    <Note keyOf="A"/>
  </div>
</template>

<script>
  import Note from './Note.vue'

  export default {
    name: "String",
    props: {
      openNote: String
    },
    components: {
      Note
    }
  }
</script>

<style scoped>

</style>

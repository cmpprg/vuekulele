<template>
  <div class="strings">
    <String openNote='A'/><br>
    <String openNote='E'/><br>
    <String openNote='C'/><br>
    <String openNote='G'/><br>
  </div>
</template>

<script>
  import String from './String'

  export default {
    name: "Neck",
    components: {
      String
    },
    data() {
      return {
        allNotes: ['A', 'A#', 'B', 'C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#']
      }
    }
  }
</script>

<style scoped>

</style>

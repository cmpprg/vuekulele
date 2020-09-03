<template>
  <div class="neck">
    <String openNote='A'/>
    <String openNote='E'/>
    <String openNote='C'/>
    <String openNote='G'/>
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
        allNotes: ['A', 'A#', 'B', 'C', 'C#', 'D',
                   'D#', 'E', 'F', 'F#', 'G', 'G#']
      }
    }
  }
</script>

<style scoped>
  .neck {
    border: 4px solid blue;
  }
</style>

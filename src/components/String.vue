<template>
  <div class="string">
    <div v-for='fret in frets' :key='fret'>
      <Note :keyOf='fret'/>
    </div>
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
    },
    data() {
      return {
        frets: ['A', 'A#', 'B', 'C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#']
      }
    }
  }
</script>

<style scoped>
  .string {
    display: block;
    padding-bottom: 40px;
  }
</style>

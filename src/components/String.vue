<template>
  <div class="string">
    <div v-for='note in orderNotesForString(openNote, allNotes)' :key='note'>
      <Note :keyOf='note'/>
    </div>
  </div>
</template>

<script>
  import Note from './Note.vue'

  export default {
    name: "String",
    props: {
      openNote: String,
    },
    components: {
      Note
    },
    data() {
      return {
        allNotes: ['A', 'A#', 'B', 'C', 'C#', 'D',
                   'D#', 'E', 'F', 'F#', 'G', 'G#']
      }
    },
    methods: {
      orderNotesForString: (startNote, collectionOfNotes) => {
        let copyNotes = [...collectionOfNotes]
        while (copyNotes[0] !== startNote) {
          copyNotes.unshift(copyNotes.pop())
        }
        return copyNotes
      }
    }
  }
</script>

<style scoped>
  .string {
    display: block;
    padding-bottom: 40px;
    height: 20px;
    width: 100%;

  }
</style>

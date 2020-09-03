<template>
  <tr class="string">
    <td v-for='note in orderNotesForString(openNote, allNotes)' :key='note'>
      <Note :keyOf='note'/>
    </td>
  </tr>
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
        allNotes: ['C4', 'C#4', 'D4', 'D#4', 'E4', 'F4',
                   'F#4', 'G4', 'G#4','A4', 'A#4', 'B4',
                   'C5', 'C#5', 'D5', 'D#5', 'E5', 'F5',
                   'F#5', 'G5', 'G#5']
      }
    },
    methods: {
      orderNotesForString: (startNote, collectionOfNotes) => {
        let copyNotes = [...collectionOfNotes]
        while (copyNotes[0] !== startNote) {
          copyNotes.unshift(copyNotes.pop())
        }
        return copyNotes.slice(0, 12)
      }
    }
  }
</script>

<style scoped>
  td {
    border-left: 2px solid 	#D3D3D3; /* white */
    border-collapse: collapse;
    font-weight:700;
  }
</style>

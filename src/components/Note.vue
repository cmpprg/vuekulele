<template>
  <div @click='playNote(keyOf)' class="note">
    <p>-------{{keyOf}}--------</p>
  </div>
</template>

<script>
  import { Synth } from 'tone'

  export default {
    name: "Note",
    props: {
      keyOf: String
    },
    methods: {
      playNote: (key) => {
        let synth = new Synth();
        synth.toMaster();
        synth.triggerAttackRelease(key, '6n')
      }
    }
  }
</script>

<style scoped>
  .note {
    text-align: center;
    background-color: #281b0d; /* light brown */
    color: 	#D3D3D3; /* white */
    padding: 10px 0px;
  }
  .note:hover {
    cursor: grab;
  }
</style>

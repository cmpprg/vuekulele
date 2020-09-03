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
        synth.triggerAttackRelease(key, '8n')
      }
    }
  }
</script>

<style scoped>
  .note {
    text-align: center;
  }
</style>

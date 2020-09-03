<template>
  <div class="neck">
    <String openNote='A4'/>
    <String openNote='E4'/>
    <String openNote='C4'/>
    <String openNote='G4'/>
  </div>
</template>

<script>
  import String from './String'

  export default {
    name: "Neck",
    components: {
      String
    }
  }
</script>

<style scoped>
  .neck {
    border: 4px solid blue;
  }
</style>

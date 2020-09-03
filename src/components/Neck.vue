<template>
  <table class="neck">
    <String openNote='A4'/>
    <String openNote='E4'/>
    <String openNote='C4'/>
    <String openNote='G4'/>
  </table>
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
    border: 4px solid #1e140a;
    border-radius: 10px;
    width: 100%;
  }

  .string-on-neck {
    border: 1px solid red
  }
</style>

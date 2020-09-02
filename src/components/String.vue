<template>
  <div class="string">
    <p>I will be the '{{openNote}}' String</p>
  </div>
</template>

<script>
  export default {
    name: "String",
    props: {
      openNote: String
    }
  }
</script>

<style scoped>

</style>

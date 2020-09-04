<template>
    <div
      class="card"
      v-bind:class="{ 'card-left': alignment === 'left',
      'card-right': alignment === 'right' }"
      >
      <p class="title">{{title}}</p>
      <p class="text">{{text}}</p>
    </div>
</template>

<script>
  export default {
    name: "Card",
    props: {
      title: String,
      text: String,
      alignment: String
    }
  }
</script>

<style scoped>
  div {
    width: 100%;
  }

  .card {
    max-width: 45%;
    min-width: 45%;
    border: 2px solid white;
    border-top-color: #281b0d;
    border-radius: 5px 5px 20px 20px;
    background-color: grey;
    color: #d4d4d4;
    font-size: 20px;
    margin-bottom: 5%;
    padding: 1% 5% 5% 5%;
  }

  .title {
    color: white;
    font-size: 30px;
    font-weight: 600;
  }
  .card-left {
    margin-left: 5%;
    float: left;
    text-align: left;
  }

  .card-right {
    margin-right: 5%;
    float: right;
    text-align: right;
  }
  .text {
    text-align: center;
  }
</style>

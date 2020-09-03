<template>
  <table class="neck">
    <tr>
      <th>OPEN</th>
      <th>1<sup>st</sup> FRET</th>
      <th>2<sup>st</sup> FRET</th>
      <th>3<sup>st</sup> FRET</th>
      <th>4<sup>st</sup> FRET</th>
      <th>5<sup>st</sup> FRET</th>
      <th>6<sup>st</sup> FRET</th>
      <th>7<sup>st</sup> FRET</th>
      <th>8<sup>st</sup> FRET</th>
      <th>9<sup>st</sup> FRET</th>
      <th>10<sup>st</sup> FRET</th>
      <th>11<sup>st</sup> FRET</th>
    </tr>

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
    background-color: #1e140a;
  }

  th {
    color: #D3D3D3;
  }
</style>

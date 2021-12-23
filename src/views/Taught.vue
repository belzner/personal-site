<template>
  <div class="taught">
    <h1>Things I've Taught</h1>
    <ul>
      <li>Linguistics</li>
      <li>Computers</li>
      <li>Other Topics</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Taught',
};
</script>

<style lang="scss" scoped>
.taught {
  min-height: 100vh;
  display: grid;
  place-content: center;
  font-family: sans-serif;
  background-color: #06d6a0;
  background-image: url('../assets/tile-06d6a0.png');
  background-position: center;
  line-height: 1;
}
</style>

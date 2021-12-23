<template>
  <div class="know">
    <h1>Things I Know</h1>
    <ul>
      <li>Education</li>
      <li>Programming Languages</li>
      <li>Other Interests</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Know',
};
</script>

<style lang="scss" scoped>
.know {
  min-height: 100vh;
  display: grid;
  place-content: center;
  font-family: sans-serif;
  background-color: #ffd166;
  background-image: url('../assets/tile-ffd166.png');
  background-position: center;
  line-height: 1;
}
</style>

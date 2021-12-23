<template>
  <div class="done">
    <h1>Things I've Done</h1>
    <ul>
      <li>Lithic</li>
      <li>Skillshare</li>
      <li>Other Work</li>
      <li>Side Projects</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Done',
};
</script>

<style lang="scss" scoped>
.done {
  min-height: 100vh;
  display: grid;
  place-content: center;
  font-family: sans-serif;
  background-color: #ef476f;
  background-image: url('../assets/tile-ef476f.png');
  background-position: center;
  line-height: 1;
}
</style>

<template>
  <div class="contact">
    <h1>Get In Touch</h1>
    <ul>
      <li>Email</li>
      <li>Linkedin</li>
      <li>Github</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Contact',
};
</script>

<style lang="scss" scoped>
.contact {
  min-height: 100vh;
  display: grid;
  place-content: center;
  font-family: sans-serif;
  background-color: #073b4c;
  background-image: url('../assets/tile-073b4c.png');
  background-position: center;
  line-height: 1;
}
</style>

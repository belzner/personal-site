<template>
  <div class="contact">
    <div class="wrapper">
      <h1 class="header">Get In Touch</h1>
      <div class="content">
        <ul>
          <li>Email</li>
          <li>Linkedin</li>
          <li>Github</li>
        </ul>
      </div>
    </div>
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
  font-family: sans-serif;
  background-color: #073b4c;
  background-image: url('../assets/tile-073b4c.png');
  background-position: center;
  line-height: 1;
}

.wrapper {
  height: 100vh;
  max-width: 1030px;
  margin: 0 auto;
  padding: 5vh;
  font-size: 16px;
}

.header {
  height: 10vh;
  color: #fff;
}

.content {
  height: 75vh;
  padding: 20px;
  background-color: rgba(255, 255, 255, 0.6);
}
</style>

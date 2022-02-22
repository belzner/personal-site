<template>
  <div id="app">
    <Intro />
    <WebDevelopment />
  </div>
</template>

<script>
import Intro from '@/views/Intro.vue';
import WebDevelopment from '@/views/WebDevelopment.vue';

export default {
  name: 'App',
  components: {
    Intro,
    WebDevelopment,
  },
};
</script>

<style lang="scss">
// Backgrounds from https://patternico.com/#uzIKpwXDPNP7Sujl
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css');
@import url('https://fonts.googleapis.com/css2?family=Chela+One&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&display=swap');

$link-color: #3d6bb5;
$link-hover-color: #6797e5;
$font-family-base: 'Open Sans', sans-serif;
$headings-font-family: 'Chela One', sans-serif;

@import '../node_modules/bootstrap/scss/bootstrap';
@import '../node_modules/bootstrap-vue/src/index.scss';

* {
  box-sizing: border-box;
}

#app {
  background-color: #118ab2;
  background-image: url('./assets/tile-118ab2.png');
  background-position: center;
}

.header {
  height: 15vh;
  max-width: 1000px;
  margin: 0 auto;
  padding: 5vh 5vh 0;
  font-size: 4rem;
}

.wrapper {
  height: 85vh;
  margin: 0 auto;
  padding: 5vh;
  position: relative;
  bottom: 0;
  display: grid;
  grid-template-rows: 1fr 1fr;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 25px;
  font-size: 1.05rem;
  line-height: 1.1rem;
}

h2 {
  font-size: 1.8rem;
  font-family: 'Arial', sans-serif;
}
</style>

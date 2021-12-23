<template>
  <div id="app">
    <Intro />
  </div>
</template>

<script>
import Intro from '@/views/Intro.vue';

export default {
  name: 'App',
  components: {
    Intro,
  },
  computed: {
    isHome() {
      return this.$route.name === 'Home';
    },
  },
};
</script>

<style lang="scss">
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css');
@import url('https://fonts.googleapis.com/css2?family=Lilita+One&display=swap');

$font-size-base: 1.4rem;
$link-color: #3d6bb5;
$link-hover-color: #6797e5;
$headings-font-family: 'Lilita One', sans-serif;

@import '../node_modules/bootstrap/scss/bootstrap';
@import '../node_modules/bootstrap-vue/src/index.scss';

* {
  box-sizing: border-box;
}
</style>

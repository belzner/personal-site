<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css');
@import url('https://fonts.googleapis.com/css2?family=Balsamiq+Sans&display=swap');

$font-size-base: 1.4rem;
$link-color: #3d6bb5;
$link-hover-color: #6797e5;
$headings-font-family: 'Balsamiq Sans', sans-serif;

@import '../node_modules/bootstrap/scss/bootstrap';
@import '../node_modules/bootstrap-vue/src/index.scss';

#app {
  text-align: center;
  height: 100vh;
}
</style>

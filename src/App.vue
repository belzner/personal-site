<template>
  <div id="app">
    <b-navbar v-if="!isHome" toggleable="lg">
      <b-navbar-brand to="/">Megan Belzner</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse">
        <template v-slot:default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-double-up"></b-icon>
          <b-icon v-else icon="chevron-double-down"></b-icon>
        </template>
      </b-navbar-toggle>

      <b-collapse id="nav-collapse" class="ml-auto" is-nav>
        <Nav />
        <Contact />
      </b-collapse>
    </b-navbar>
    <router-view/>
  </div>
</template>

<script>
import Nav from './components/Nav.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    Nav,
    Contact,
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

  .navbar-brand {
    font-family: $headings-font-family;
  }

  .navbar-expand {
    justify-content: space-between;
  }

  .navbar-collapse {
    flex-grow: 0;
  }
}
</style>

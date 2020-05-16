<template>
  <b-navbar-nav>
    <b-navbar-item class="mx-2">👩‍💻 <router-link to="/about">About</router-link></b-navbar-item>
    <b-navbar-item class="mx-2">🏢 <router-link to="/work">Work</router-link></b-navbar-item>
    <b-navbar-item class="mx-2">📝 <router-link to="/teaching">Teaching</router-link></b-navbar-item>
    <b-navbar-item class="mx-2">🎨 <router-link to="/projects">Projects</router-link></b-navbar-item>
  </b-navbar-nav>
</template>

<style lang="scss" scoped>
.router-link-exact-active {
  color: #6797e5;
  text-decoration: underline;
}
</style>

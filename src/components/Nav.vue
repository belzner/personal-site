<template>
  <div class="nav">
    <span class="nav-item">👩‍💻 <router-link to="/about">About</router-link></span>
    <span class="nav-item">🏢 <router-link to="/work">Work</router-link></span>
    <span class="nav-item">📝 <router-link to="/teaching">Teaching</router-link></span>
    <span class="nav-item">🎨 <router-link to="/projects">Projects</router-link></span>
  </div>
</template>

<style lang="scss" scoped>
.nav-item {
  margin: 0 10px;
}
</style>

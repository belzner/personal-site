<template>
  <div class="home">
    <b-avatar src="../assets/avatar.png" size="200px" class="avatar"></b-avatar>
    <h1>Megan Belzner</h1>
    <Nav />
    <Contact />
  </div>
</template>

<script>
import Nav from '../components/Nav.vue';
import Contact from '../components/Contact.vue';

export default {
  name: 'Home',
  components: {
    Nav,
    Contact,
  },
};
</script>

<style lang="scss" scoped>
.home {
  height: 100%;
  padding-bottom: 50px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  h1 {
    margin: 20px;
  }
}
</style>

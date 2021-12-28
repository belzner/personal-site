<template>
  <div class="contact">
    <h1 class="header">Get In Touch</h1>
    <div class="wrapper">
      <InfoCard :can-flip="false">
        <template v-slot:header>
          <h2>Email</h2>
        </template>
      </InfoCard>
      <InfoCard :can-flip="false">
        <template v-slot:header>
          <h2>LinkedIn</h2>
        </template>
      </InfoCard>
      <InfoCard :can-flip="false">
        <template v-slot:header>
          <h2>Twitter</h2>
        </template>
      </InfoCard>
      <InfoCard :can-flip="false">
        <template v-slot:header>
          <h2>Github</h2>
        </template>
      </InfoCard>
    </div>
  </div>
</template>

<script>
import InfoCard from '@/components/InfoCard.vue';

export default {
  name: 'Contact',
  components: {
    InfoCard,
  },
};
</script>

<style lang="scss" scoped>
.contact {
  height: 100vh;
  background-color: #073b4c;
  background-image: url('../assets/tile-073b4c.png');
  background-position: center;
  line-height: 1;
}

.header {
  color: #fff;
}

.wrapper {
  grid-template-columns: 1fr 1fr;
}
</style>

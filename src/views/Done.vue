<template>
  <div class="done">
    <h1 class="header">Things I've Done</h1>
    <div class="wrapper">
      <InfoCard>
        <template v-slot:header>
          <h2>Lithic</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Skillshare</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Internships</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>MIT</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>ESP</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Projects</h2>
        </template>
      </InfoCard>
    </div>
  </div>
</template>

<script>
import InfoCard from '@/components/InfoCard.vue';

export default {
  name: 'Done',
  components: {
    InfoCard,
  },
};
</script>

<style lang="scss" scoped>
.done {
  height: 100vh;
  background-color: #ef476f;
  background-image: url('../assets/tile-ef476f.png');
  background-position: center;
  line-height: 1;
}
</style>

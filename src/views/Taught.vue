<template>
  <div class="taught">
    <h1 class="header">Things I've Taught</h1>
    <div class="wrapper">
      <InfoCard>
        <template v-slot:header>
          <h2>Class 1</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Class 2</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Class 3</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Class 4</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Class 5</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>And More</h2>
        </template>
      </InfoCard>
    </div>
  </div>
</template>

<script>
import InfoCard from '@/components/InfoCard.vue';

export default {
  name: 'Taught',
  components: {
    InfoCard,
  },
};
</script>

<style lang="scss" scoped>
.taught {
  height: 100vh;
  background-color: #06d6a0;
  background-image: url('../assets/tile-06d6a0.png');
  background-position: center;
  line-height: 1;
}
</style>

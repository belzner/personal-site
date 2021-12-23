<template>
  <div class="taught">
    <TabContainer header="Things I've Taught">
      <b-tab title="Linguistics">
        <div>Linguistics</div>
      </b-tab>
      <b-tab title="Computers">
        <div>Computers</div>
      </b-tab>
      <b-tab title="Other Topics">
        <div>Other Topics</div>
      </b-tab>
    </TabContainer>
  </div>
</template>

<script>
import TabContainer from '@/components/TabContainer.vue';

export default {
  name: 'Taught',
  components: {
    TabContainer,
  },
};
</script>

<style lang="scss" scoped>
.taught {
  min-height: 100vh;
  font-family: sans-serif;
  background-color: #06d6a0;
  background-image: url('../assets/tile-06d6a0.png');
  background-position: center;
  line-height: 1;
}
</style>

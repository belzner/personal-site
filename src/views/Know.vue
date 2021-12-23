<template>
  <div class="know">
    <TabContainer header="Things I Know">
      <b-tab title="Programming Languages">
        <div>Programming Languages</div>
      </b-tab>
      <b-tab title="Education">
        <div>Education</div>
      </b-tab>
      <b-tab title="Other Interests">
        <div>Other Interests</div>
      </b-tab>
    </TabContainer>
  </div>
</template>

<script>
import TabContainer from '@/components/TabContainer.vue';

export default {
  name: 'Know',
  components: {
    TabContainer,
  },
};
</script>

<style lang="scss" scoped>
.know {
  min-height: 100vh;
  font-family: sans-serif;
  background-color: #ffd166;
  background-image: url('../assets/tile-ffd166.png');
  background-position: center;
  line-height: 1;
}
</style>

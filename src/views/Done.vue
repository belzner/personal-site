<template>
  <div class="done">
    <TabContainer header="Things I've Done">
      <b-tab title="Lithic">
        <div>Lithic</div>
      </b-tab>
      <b-tab title="Skillshare">
        <div>Skillshare</div>
      </b-tab>
      <b-tab title="Other Work">
        <div>Other Work</div>
      </b-tab>
      <b-tab title="Side Projects">
        <div>Side Projects</div>
      </b-tab>
    </TabContainer>
  </div>
</template>

<script>
import TabContainer from '@/components/TabContainer.vue';

export default {
  name: 'Done',
  components: {
    TabContainer,
  },
};
</script>

<style lang="scss" scoped>
.done {
  min-height: 100vh;
  font-family: sans-serif;
  background-color: #ef476f;
  background-image: url('../assets/tile-ef476f.png');
  background-position: center;
  line-height: 1;
}
</style>

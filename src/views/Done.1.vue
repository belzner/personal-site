<template>
  <div class="done">
    <TabContainer header="Things I've Done">
      <b-tab title="Lithic">
        <div>Lithic</div>
      </b-tab>
      <b-tab title="Skillshare">
        <p>
          Skillshare is an online learning community for creatives with classes in illustration, design, photography, video, and more. I worked there
          from July 2016 to November 2018, as a full-stack software engineer and (starting from late 2017/early 2018) as the tech lead for the Core Experience
          team (focused on central product features for finding, taking, and teaching classes).
        </p>
        <p>
          During my time at Skillshare, I led projects such as building the architecture for selling memberships in multiple currencies and testing different
          price points, overhauling the logic for the class search feature to better surface relevant classes, and creating external APIs for use by B2B
          clients wanting more direct access to data on classes and on their employees' use of the platform.
        </p>
        <p>
          In addition to these and other projects, I helped to start an engineering apprenticeship program, assisting with hiring and mentorship of the first
          apprentice (who ultimately accepted a full-time offer). I also assisted in the due diligence process for the company's Series C fundraise.
        </p>
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

<template>
  <div class="know">
    <TabContainer header="Things I Know">
      <b-tab title="Programming">
        <p>
          <span class="emphasize">Javascript</span> is my language of choice, on both the frontend and backend.
          I've worked with Typescript and vanilla Javascript (and a bit of Coffeescript!) and a wide variety of
          frameworks (Vue, React and React Native, AngularJS, Backbone).
        </p>
        <p>
          Besides Javascript, I've worked extensively with <span class="emphasize">HTML</span>,
          <span class="emphasize">CSS</span>, <span class="emphasize">PHP</span>, and <span class="emphasize">SQL</span>
          and occasionally with <span class="emphasize">Python</span> and <span class="emphasize">C++</span>.
          I love working across the stack, picking up new things, and understanding systems from button click to database call.
        </p>
        <p>
          In school and hobbies, I've tried out a huge range of other languages. I learned <span class="emphasize">StarLogo</span>,
          <span class="emphasize">NetLogo</span>, and <span class="emphasize">Matlab</span> in high school, and
          <span class="emphasize">Objective-C</span> and <span class="emphasize">LaTeX</span> at summer programs. In college,
          I learned <span class="emphasize">Bluespec System Verilog</span> and a bit of <span class="emphasize">Assembly</span>
          for a processor design class, and a bit of <span class="emphasize">Scheme</span> as well.
        </p>
      </b-tab>
      <b-tab title="Education">
        <p>
          I graduated from MIT with a Bachelor of Science in Computer Science and Engineering in 2016.
        </p>
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

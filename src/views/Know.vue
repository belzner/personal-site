<template>
  <div class="know">
    <TabContainer header="Things I Know">
      <b-tab title="Programming">
        <p>
          <span class="emphasize">Javascript</span> is my language of choice, on both the frontend and backend. I've worked with Typescript and
          vanilla Javascript (and a bit of Coffeescript!) and a wide variety of frameworks (Vue, React and React Native, AngularJS, Backbone).
        </p>
        <p>
          Besides Javascript, I've worked extensively with <span class="emphasize">HTML</span>, <span class="emphasize">CSS</span>,
          <span class="emphasize">PHP</span>, and <span class="emphasize">SQL</span>, and occasionally with <span class="emphasize">Python</span>
          and <span class="emphasize">C++</span>. I love working across the stack, picking up new things, and understanding systems from button click
          to database call.
        </p>
        <p>
          In school and hobbies, I've tried out a huge range of other languages. I learned <span class="emphasize">StarLogo</span>,
          <span class="emphasize">NetLogo</span>, and <span class="emphasize">Matlab</span> in high school, and <span class="emphasize">Objective-C</span>
          and <span class="emphasize">LaTeX</span> at summer programs. In college, I learned <span class="emphasize">Bluespec System Verilog</span>
          and a bit of <span class="emphasize">Assembly</span> for a processor design class, and a bit of <span class="emphasize">Scheme</span> as well.
        </p>
      </b-tab>
      <b-tab title="Education">
        <p>
          I graduated from MIT with a Bachelor of Science in Computer Science and Engineering in 2016. Within my degree, I took a wide variety of
          classes on topics from AI (<span class="emphasize">6.034</span> Artificial Intelligence, <span class="emphasize">6.803</span>
          The Human Intelligence Enterprise) to processor design (<span class="emphasize">6.004</span> Computation Structures,
          <span class="emphasize">6.175</span> Constructive Computer Architecture) to UI design (<span class="emphasize">6.813</span>
          User Interface Design and Implementation) to systems (<span class="emphasize">6.033</span> Computer System Engineering) and security
          (<span class="emphasize">6.858</span> Computer Systems Security).
        </p>
        <p>
          Outside of CS, I took classes in areas such as linguistics (<span class="emphasize">24.900</span> Introduction to Linguistics,
          <span class="emphasize">24.901</span> Language and Structure I: Phonology, <span class="emphasize">24.902</span> Language and Structure II: Syntax,
          <span class="emphasize">24.903</span> Language and Structure III: Semantics, <span class="emphasize">24.914</span> Language Variation and Change),
          media studies (<span class="emphasize">21W.737</span> 21st Century Journalism, <span class="emphasize">CMS.614</span> Network Cultures),
          philosophy (<span class="emphasize">24.09</span> Minds and Machines), intellectual property law (<span class="emphasize">6.903</span> Patents,
          Copyrights, and the Law of Intellectual Property), and acting (<span class="emphasize">21M.600</span> Introduction to Acting).
        </p>
      </b-tab>
      <b-tab title="Other Interests">
        <p>
          I'm fascinated by <span class="emphasize">how people communicate over digital media</span>. I can tell you about how emojis get created and
          how they get used, the tricks we use to communicate tone in informal writing, and how memes have changed over time.
        </p>
        <p>
          In high school I started an extensive worldbuilding project, including a full <span class="emphasize">constructed language</span> designed from scratch.
          Although this particular project fell by the wayside, I've continued to grow my familiarity with language construction techniques and returned to
          the idea here and there.
        </p>
        <p>
          For more relaxed hobbies, I watch a lot of <span class="emphasize">highly-researched video essays</span> on YouTube (especially on topics like
          game design and media) and play far too much <span class="emphasize">Sims 4</span>.
        </p>
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

<template>
  <div class="know">
    <h1 class="header">Things I Know</h1>
    <div class="wrapper">
      <InfoCard name="js">
        <template v-slot:header>
          <h2>Javascript, HTML, &amp; CSS</h2>
        </template>
        <template v-slot:content>
          <p>My love of coding started with my first introduction to HTML on Neopets, and exploded from there.</p>
          <p>These days Javascript (or Typescript!) is my language of choice for both frontend and backend.</p>
          <p>I'm a fan of Vue, but I've also worked with React (and React Native), AngularJS, and Backbone.</p>
        </template>
      </InfoCard>
      <InfoCard name="others">
        <template v-slot:header>
          <h2>PHP, SQL, Python, C++, Scheme, Assembly, LaTeX...</h2>
        </template>
        <template v-slot:content>
          <p>I'm firmly a full-stack engineer, and love being able to follow a user action from button click to database call.</p>
          <p>Besides Javascript, I've worked professionally with PHP, SQL, Python, and C++.</p>
          <p>Outside of work I've tried out a huge range of languages, from Matlab to Objective-C to Scheme.</p>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Linguistics</h2>
        </template>
        <template v-slot:content>
          <p>I've always found language structures fascinating, and if not for CS, I likely would have majored in linguistics.</p>
          <p>These days it's still one of my favorite topics for books and podcasts.</p>
          <p>I also love to notice and think about linguistic phenomena in the real world.</p>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Emoji</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Internet Culture</h2>
        </template>
      </InfoCard>
      <InfoCard>
        <template v-slot:header>
          <h2>Pok&eacute;mon</h2>
        </template>
      </InfoCard>
    </div>
  </div>
</template>

<script>
import InfoCard from '@/components/InfoCard.vue';

export default {
  name: 'Know',
  components: {
    InfoCard,
  },
};
</script>

<style lang="scss" scoped>
.know {
  height: 100vh;
  background-color: #ffd166;
  background-image: url('../assets/tile-ffd166.png');
  background-position: center;
  line-height: 1;
}

.header {
  height: 15vh;
  max-width: 1000px;
  margin: 0 auto;
  padding: 5vh 5vh 0;
  font-size: 4rem;
}

.wrapper {
  height: 85vh;
  max-width: 1000px;
  margin: 0 auto;
  padding: 5vh;
  position: relative;
  bottom: 0;
  display: grid;
  grid-template-rows: 1fr 1fr;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 25px;
  font-size: 1.05rem;
  line-height: 1.1rem;
}

h2 {
  font-size: 1.8rem;
  font-family: 'Arial', sans-serif;
}
</style>

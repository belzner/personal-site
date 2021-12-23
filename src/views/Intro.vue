<template>
  <div class="intro">
    <h1 @mouseover="triggerAnim" ref="wave">
      <span
        v-for="(char, idx) in headerText"
        :key="'header-' + idx"
        :data-text="char"
        :class="{ space: char === ' ', sticker: char !== ' ' }"
        :style="{
          color: gradientColors[getIdxWithoutSpace(idx) % gradientColors.length],
          '--anim-delay': (getIdxWithoutSpace(idx) / 10) + 's',
        }"
      >
        <span>{{ char }}</span>
      </span>
    </h1>
  </div>
</template>

<script>
export default {
  name: 'Intro',
  data() {
    return {
      headerText: 'Hi, I\'m Megan',
      gradientColors: ['#e2bef1', '#f5cdde', '#f9ded7', '#fbf7d5', '#c6f8e5', '#cce1f2'],
    };
  },
  methods: {
    getIdxWithoutSpace(idx) {
      const spaces = this.headerText.slice(0, idx).split(' ').length - 1;
      return idx - spaces;
    },
    triggerAnim() {
      if (this.$refs.wave.classList.contains('wave-anim')) {
        return;
      }
      this.$refs.wave.classList.add('wave-anim');
      const animSeconds = (this.getIdxWithoutSpace(this.headerText.length - 1) / 10) + 1;
      setTimeout(() => this.$refs.wave.classList.remove('wave-anim'), animSeconds * 1000);
    },
  },
};
</script>

<style lang="scss" scoped>
.intro {
  min-height: 100vh;
  min-height: -webkit-fill-available;
  display: grid;
  place-content: center;
  font-family: sans-serif;
  background-color: #327ddf;
  background-image: url('../assets/tile-blue.png');
  background-position: center;
  line-height: 1;
}

@keyframes bounce {
  0% {
    transform: translateY(0em) rotate3d(0);
  }

  50% {
    transform: translateY(-0.3em) rotate3d(1, 0, 0, 25deg);
  }

  100% {
    transform: translateY(0em) rotate3d(0);
  }
}

@keyframes liftShadow {
  0% {
    text-shadow: 0.08em 0.08em 0.05em rgba(0, 0, 0, 0.75),
      -0.07em -0.05em 0.05em rgba(0, 0, 0, 0.75);
  }

  50% {
    text-shadow: 0.08em 0.38em 0.1em rgba(0, 0, 0, 0.25);
  }

  100% {
    text-shadow: 0.08em 0.08em 0.05em rgba(0, 0, 0, 0.75),
      -0.07em -0.05em 0.05em rgba(0, 0, 0, 0.75);
  }
}

.wave-anim {
  .sticker {
    animation-duration: 1s;
    animation-name: bounce;

    &::before {
      animation-duration: 1s;
      animation-name: liftShadow;
    }
  }
}

.sticker {
  --anim-delay: 0s;
  display: inline-grid;
  grid-template-areas: "text";
  place-items: center;
  font-weight: 700;
  font-size: 7rem;
  letter-spacing: 0.17em;
  animation-delay: var(--anim-delay);

  span {
    -webkit-text-stroke: 0.01em rgba(0, 0, 0, 0.6);
  }

  & > *,
  &::before {
    grid-area: text;
  }

  &::before {
    content: attr(data-text);
    color: #fff;
  }

  &::before {
    animation-delay: var(--anim-delay);
    -webkit-text-stroke: 0.21em white;
    text-shadow: 0.08em 0.08em 0.05em rgba(0, 0, 0, 0.75),
      -0.07em -0.05em 0.05em rgba(0, 0, 0, 0.75);
  }
}

.space {
  display: inline-block;
  width: 0.5em;
}
</style>

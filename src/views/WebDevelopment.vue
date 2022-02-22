<template>
  <div class="web-development">
    <div class="anim-wrapper">
      <div class="webpage-container">
        <div class="webpage-green-square"></div>
        <div class="webpage-blue-square"></div>
      </div>
    </div>
    <div class="content">
      From my first introduction to HTML on Neopets in middle school, I was hooked.
    </div>
  </div>
</template>

<script>
export default {
  name: 'WebDevelopment',
  components: {},
};
</script>

<style lang="scss" scoped>
.web-development {
  padding: 100px;
  line-height: 1;
  display: flex;
}

.content {
  background-color: rgba(255, 255, 255, 0.8);
  flex-grow: 1;
  position: relative;
  top: 20px;
  padding: 30px;
  margin-right: 20px;
  border-radius: 0.5em;
}

.anim-wrapper {
  perspective: 1000px;
}

@keyframes bounceOuter {
  0% {
    transform: rotate(-80deg) rotate3d(0, 1, 0, 60deg);
    box-shadow: -0.38em 0.08em 0.2em rgba(0, 0, 0, 0.25);
  }

  50% {
    transform: rotate(-80deg) rotate3d(0, 1, 0, 60deg) translateZ(1.5em);
    box-shadow: -3.38em 0.38em 1em rgba(0, 0, 0, 0.25);
  }

  100% {
    transform: rotate(-80deg) rotate3d(0, 1, 0, 60deg);
    box-shadow: -0.38em 0.08em 0.2em rgba(0, 0, 0, 0.25);
  }
}

@keyframes bounceInner {
  0% {
    transform: translateZ(0);
    box-shadow: -0.38em 0.08em 0.2em rgba(0, 0, 0, 0.25);
  }

  50% {
    transform: translateZ(0.5em);
    box-shadow: -1.38em 0.38em 1em rgba(0, 0, 0, 0.25);
  }

  100% {
    transform: translateZ(0);
    box-shadow: -0.38em 0.08em 0.2em rgba(0, 0, 0, 0.25);
  }
}

.webpage-container {
  transform-style: preserve-3d;
  background-image: url('../assets/webpage-base.png');
  background-size: contain;
  border-radius: 0.5em;
  width: 400px;
  height: 245px;
  animation-duration: 4s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  // animation-play-state: paused;
  animation-name: bounceOuter;

  .webpage-green-square, .webpage-blue-square {
    position: absolute;
    animation-duration: 4s;
    animation-iteration-count: infinite;
    animation-timing-function: ease-in-out;
    // animation-play-state: paused;
    animation-name: bounceInner;
  }

  .webpage-green-square {
    top: 45px;
    left: 20px;
    width: 75px;
    height: 180px;
    background-color: #c6f8e5;
    animation-delay: -1s;
  }

  .webpage-blue-square {
    top: 85px;
    left: 275px;
    width: 105px;
    height: 95px;
    background-color: #cce1f2;
    animation-delay: -3s;
  }

  &:hover {
    animation-play-state: running;

    .webpage-green-square, .webpage-blue-square {
      animation-play-state: running;
    }
  }
}
</style>

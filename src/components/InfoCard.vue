<template>
  <div class="info-card"
    @click="flip()"
    @mouseover="hover(true)"
    @mouseout="hover(false)"
    ref="card"
  >
    <div class="front">
      <slot name="header"><div></div></slot>
    </div>
    <div class="back">
      <slot name="content"><div></div></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Know',
  props: {
    canFlip: {
      type: Boolean,
      default: true,
    },
  },
  methods: {
    flip() {
      if (!this.canFlip) {
        return;
      }
      this.$refs.card.classList.toggle('flipped');
    },
    hover(isHover) {
      this.$refs.card.children.forEach((child) => {
        if (isHover) {
          child.classList.add('hover');
        } else {
          child.classList.remove('hover');
        }
      });
    },
  },
};
</script>

<style lang="scss" scoped>
.info-card {
  position: relative;

  .front, .back {
    position: absolute;
    backface-visibility: hidden;
    transition: transform 0.5s;
    background-color: rgba(255, 255, 255, 0.6);
    width: 100%;
    height: 100%;
    padding: 15px;
    overflow: auto;
    cursor: pointer;
    box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.4);
    transition: transform 0.5s, box-shadow 0.5s;

    &.hover {
      transform: translate(-5px, -7px) scale(1.02) rotateZ(0.5deg);
      box-shadow: 8px 10px 8px rgba(0, 0, 0, 0.15);
    }
  }

  .back {
    transform: rotateY(-180deg);

    &.hover {
      transform: rotateY(-180deg) translate(-5px, -7px) scale(1.02) rotateZ(0.5deg);
    }
  }

  &.flipped {
    .front {
      transform: rotateY(180deg);

      &.hover {
        transform: rotateY(180deg) translate(-5px, -7px) scale(1.02) rotateZ(0.5deg);
      }
    }

    .back {
      transform: rotateY(0deg);

      &.hover {
        transform: rotateY(0deg) translate(-5px, -7px) scale(1.02) rotateZ(0.5deg);
      }
    }
  }
}
</style>

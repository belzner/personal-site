<template>
  <div class="wrapper">
    <h1 class="header">{{ header }}</h1>
    <b-tabs pills vertical nav-wrapper-class="tab-column" content-class="content-column">
      <slot></slot>
    </b-tabs>
  </div>
</template>

<script>
export default {
  name: 'TabContainer',
  props: {
    header: String,
  },
};
</script>

<style lang="scss" scoped>
.wrapper {
  height: 100vh;
  max-width: 1000px;
  margin: 0 auto;
  padding: 5vh;
  font-size: 16px;
}

.header {
  height: 10vh;
}

/deep/ .tabs {
  height: 75vh;
}

/deep/ .tab-column {
  background-color: rgba(255, 255, 255, 0.6);
  margin-right: 30px;
  padding: 20px;
  width: 200px;

  .nav-pills .nav-link {
    color: #000;
  }

  .nav-pills .nav-link:hover {
    color: rgba(0, 0, 0, 0.6);
  }

  .nav-pills .nav-link.active {
    background-color: rgba(0, 0, 0, 0.3);
    color: #fff;
  }
}

/deep/ .content-column {
  background-color: rgba(255, 255, 255, 0.6);
  padding: 20px;
}
</style>

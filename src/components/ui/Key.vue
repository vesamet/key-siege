<template>
  <div class="container">
    <div class="side"></div>
    <div class="top">
      <img v-if="imgSrc" :src="imgSrc" :alt="shortcut" class="icon" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imgSrc: {
      type: String,
      default: ""
    },
    shortcut: {
      type: String,
      default: ""
    }
  }
};
</script>

<style lang="scss" scoped>
.container {
  width: 60px;
  height: 60px;
  position: relative;
}
.side {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: var(--primary);
  clip-path: polygon(
    21% 6%,
    76% 6%,
    84% 9%,
    88% 15%,
    100% 100%,
    0 100%,
    11% 15%,
    14% 9%
  );
  border-radius: 4px;
}
.top {
  position: absolute;
  top: 0;
  left: 50%;
  transform: translate(-50%, 0%);
  text-align: center;
  border-radius: 10px;
  background-color: var(--primary-light);
  width: 45px;
  height: 45px;
  z-index: 1;
  padding: 5px;
}
.icon {
  width: 100%;
  position: relative;
  z-index: 2;
}
</style>

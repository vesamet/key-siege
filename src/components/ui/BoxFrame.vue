<template>
  <div class="container">
    <div class="bevel top"></div>
    <div class="bevel side"></div>
    <div class="bevel ornate"></div>
    <div class="content"><slot /></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  background-color: var(--secondary);
  border-radius: 15px;
  position: relative;
  z-index: 0;
  min-height: 100px;
  box-shadow: 0px 0px 10px var(--primary);
}
.bevel {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.top {
  z-index: 3;
  border-radius: 15px;
  border: 10px solid var(--primary);
  top: -4px;
  left: -4px;
}
.side {
  z-index: 2;
  border-radius: 15px;
  border: 10px solid var(--primary-light);
}
.content {
  position: absolute;
  top: 0;
  left: 0;
  padding: 13px;
  z-index: 1;
  width: 100%;
  height: 100%;
}
</style>

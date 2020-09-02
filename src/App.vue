<template>
  <div class="main-container">
    <div class="pure-g">
      <div class="pure-u-1 pure-u-md-1-2">
        <BoxFrame class="main-box-frame">d</BoxFrame>
      </div>
      <div class="pure-u-1 pure-u-md-1-2">
        <BoxFrame class="main-box-frame">d</BoxFrame>
      </div>
    </div>
  </div>
</template>

<script>
import BoxFrame from "@/components/ui/BoxFrame.vue";
export default {
  name: "App",
  components: {
    BoxFrame
  }
};
</script>

<style lang="scss">
html,
body {
  width: 100%;
  height: 100%;
  margin: 0px;
  padding: 0px;
}
.main-container {
  width: 100%;
  height: 100%;
  background-color: var(--light);
}
.main-box-frame {
  margin: 10px;
}
</style>

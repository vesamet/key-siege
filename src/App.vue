<template>
  <div class="main-container">
    <div class="main-centered">
      <div class="pure-g">
        <div class="pure-u-1 pure-u-md-1-2">
          <BoxFrame class="main-box-frame">
            <ActionBar />
          </BoxFrame>
        </div>
        <div class="pure-u-1 pure-u-md-1-2">
          <BoxFrame class="main-box-frame">d</BoxFrame>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BoxFrame from "@/components/ui/BoxFrame.vue";
import ActionBar from "@/components/ActionBar.vue";
export default {
  name: "App",
  components: {
    BoxFrame,
    ActionBar
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
  background-color: var(--light);
  font-size: $body-font;
}
.main-container {
  @include vertical-center;
  margin: auto;
  max-width: 900px;
  text-align: center;
}
.main-box-frame {
  margin: 10px;
}
</style>

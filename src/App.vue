<template>
  <div>
    <it-main-wrapper></it-main-wrapper>
  </div>
</template>

<script>
import itMainWrapper from "./components/it-main-wrapper.vue";

export default {
  name: "App",
  components: {
    itMainWrapper,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<template>
  <div>
    <it-catalog></it-catalog>
    <it-cart></it-cart>
  </div>
</template>

<script>
import itCatalog from "./it-catalog.vue";
import itCart from "./it-cart.vue";

export default {
  name: "it-main-wrapper",
  components: {
    itCatalog,
    itCart,
  },
};
</script>
<style lang="scss"></style>

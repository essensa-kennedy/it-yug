<template>
  <div class="catalog">
    <it-catalog-item></it-catalog-item>
    <it-catalog-item></it-catalog-item>
    <it-catalog-item></it-catalog-item>
  </div>
</template>

<script>
import itCatalogItem from "./it-catalog-item.vue";

export default {
  name: "it-catalog",
  components: {
    itCatalogItem,
  },
};
</script>
<style lang="scss"></style>

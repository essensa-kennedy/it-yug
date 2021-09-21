<template>
  <div class="container">
    <div class="catalog">
      <it-catalog-item></it-catalog-item>
      <it-catalog-item></it-catalog-item>
      <it-catalog-item></it-catalog-item>
    </div>
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
<style lang="scss">
.catalog {
  display: flex;
}
</style>

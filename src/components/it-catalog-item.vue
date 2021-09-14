<template>
  <div class="item">
    <div class="item__picture">
      <img class="picture-item" src="" alt="" />
    </div>
    <div class="item__sale">скидка на комплект</div>
    <div class="item__rating">
      <div class="item__stars"><span>4.9</span></div>
      <div class="item__reviews">13 отзывов</div>
    </div>
    <div class="item__title">Принтер Brother MFC-1123</div>
    <div class="item__details">чёрный, А4</div>
    <div class="item__status"><span>в наличии</span></div>
    <div class="item__price-section">
      <div class="item__price">32 999 руб.</div>
      <button class="add"><span>+</span></button>
    </div>
  </div>
</template>

<script>
export default {
  name: "it-catalog-item",
};
</script>
<style lang="scss">
.add {
  background-color: $accentColor;
}
</style>

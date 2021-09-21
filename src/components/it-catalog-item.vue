<template>
  <div class="item">
    <div class="item__picture">
      <img class="picture-item" src="../img/photo.png" alt="" />
    </div>
    <div class="item__sale">скидка на комплект</div>
    <div class="item__rating">
      <div class="item__icon">
        <span
          ><svg
            width="22"
            height="22"
            viewBox="0 0 22 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g id="star">
              <path
                id="Star 1"
                d="M11 0L13.4697 7.60081H21.4616L14.996 12.2984L17.4656 19.8992L11 15.2016L4.53436 19.8992L7.00402 12.2984L0.538379 7.60081H8.53035L11 0Z"
                fill="#67A513"
              />
            </g></svg
        ></span>
      </div>
      <div class="item__stars"><span>4.9</span></div>
      <div class="item__reviews">13 отзывов</div>
    </div>
    <div class="item__title">Принтер Brother MFC-1123</div>
    <div class="item__details">чёрный, А4</div>
    <div class="item__status">
      <div class="item__status-icon">
        <span
          ><svg
            width="16"
            height="13"
            viewBox="0 0 16 13"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g id="Frame 115">
              <g id="Group 24">
                <path
                  id="yes"
                  d="M3 6.5L6.33427 10L13 3"
                  stroke="#8FBF4D"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </g>
            </g></svg
        ></span>
      </div>
      <span>в наличии</span>
    </div>
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
.item {
  width: 290px;
  height: 445px;
  background-color: #f2f5f7;
  margin-left: 20px;
  position: relative;
  display: flex;
  flex-direction: column;
  padding: 35px 25px 0px 25px;

  &__picture {
  }
  &__sale {
    position: absolute;
    @include secondFont;
    font-weight: 400;
    font-size: 15px;
    background-color: $darkColor;
    color: $whiteColor;
    opacity: 0.7;
    padding: 10px 10px 10px 10px;
    top: 20px;
    left: 20px;
  }
  &__rating {
    align-self: flex-start;
    display: flex;
    align-items: center;
    margin-top: 15px;
  }
  &__stars span {
    color: $accentColor;
    @include mainFont;
    font-weight: 500;
    font-size: 20px;
    line-height: 140%;
  }
  &__reviews {
    @include mainFont;
    font-size: 13px;
    opacity: 0.5;
    margin-left: 5px;
  }
  &__title {
    align-self: flex-start;
    @include mainFont;
    color: &darkColor;
    font-weight: 700;
    font-size: 17px;
    line-height: 140%;
  }
  &__details {
    align-self: flex-start;
    color: $textColor;
    margin-top: 5px;
    font-weight: normal;
    font-size: 17px;
    line-height: 140%;
  }
  &__status {
    flex: 1 1 auto;
    display: flex;
    color: #b6c4a3;
    margin-top: 5px;
    font-weight: normal;
    font-size: 15px;
    line-height: 140%;
    @include secondFont;
  }
  &__price-section {
    display: flex;
    margin-bottom: 20px;
    align-items: center;
    justify-content: space-between;
  }
  &__price {
    font-style: normal;
    font-weight: bold;
    font-size: 24px;
    line-height: 140%;
  }
}

.item:first-child {
  margin-left: 0;
}

.add {
  background: linear-gradient(79.29deg, #8fbf4d 10.81%, #7cb72c 52.15%);
  color: $whiteColor;
  width: 62px;
  height: 62px;
  border-radius: 50%;
}

.add span::before {
  display: inline-block;
  content: "";
  width: 60px;
  height: 60px;
  background: url(../img/svg/buy.svg) center center no-repeat;
}
</style>

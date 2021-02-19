<template>
  <div class="our-product">
    <h2 class="our-product__title">Our products</h2>
    <div class="our-product__block">
      <ul class="our-product__list">
        <li class="our-product__item">
          <div class="our-product__box">
            <h5 class="our-product__name">Derma Roller</h5>
            <the-link>Learn more</the-link>
          </div>
          <p class="our-product__content">
            <span>Derma Rolling therapy</span> is a salon procedure loved by
            millions of women across the world. It has been proven to be
            effective for natural skin recovery.
          </p>
        </li>
        <!-- <li class="our-product__item">
                  <div class="our-product__box">
                      <h5 class="our-product__name"></h5>
                  </div>
                  <p class="our-product__content"></p>
              </li>
              <li class="our-product__item">
                  <div class="our-product__box">
                      <h5 class="our-product__name"></h5>
                  </div>
                  <p class="our-product__content"></p>
              </li> -->
      </ul>
    </div>
    <div class="our-product__buttons">
      <button class="our-product__btn">&#8249;</button>
      <button class="our-product__btn">&#8250;</button>
    </div>
  </div>
</template>

<script>
import TheLink from "./common/TheLink.vue";
export default {
  name: "The-our-product",
  components: { TheLink },
};
</script>

<style lang="scss">
.our-product {
  padding: 0 20%;
  margin-bottom: 117px;
  position: relative;
  &:after {
    content: url("../assets/IMG_0182-removebg-preview.png");
    position: absolute;
    top: -306px;
    right: 8%;
  }
  &__title {
    margin-bottom: 75px;
    @include text($H720, 900, $dark-color) {
      line-height: 74px;
      letter-spacing: 2px;
      text-transform: capitalize;
    }
  }
  &__block {
    margin-bottom: 25px;
  }
  &__item {
    margin-left: 39px;
  }
  &__box {
    margin-bottom: 38px;
    @include flex(flex-start, center);
  }
  &__name {
    margin-right: 94px;
    @include text($H360, 900, $dark-color) {
      line-height: 37px;
      letter-spacing: 1px;
      text-transform: capitalize;
    }
  }
  &__content {
    max-width: 500px;
    @include text($H80, 500, $black-color) {
      line-height: 30px;
      letter-spacing: 0.5px;
    }
    span {
      font-style: italic;
      font-weight: 900;
    }
  }
  &__btn {
    background-color: $pink-btn;
    border: 1px solid #a6a8a9;
    outline: none;
    cursor: pointer;
    padding: 15px 15px 14px 17px;
    border-radius: 50% 75%;
    color: #a6a8a9;
    @include transition(background-color);
    &:hover {
      background-color: $pink-color;
    }
    &:active {
      background-color: #d6bfcb;
    }
    &:not(last-child) {
      margin-right: 24px;
    }
  }
}
</style>

<template>
  <div class="our-product">
    <h2 class="our-product__title">Our products</h2>
    <div class="our-product__box">
      <ul class="our-product__list">
        <li class="our-product__item">
          <div class="our-product__box">
            <h5 class="our-product__name">Derma Roller</h5>
            <the-link>Learn more</the-link>
          </div>
          <p class="our-product__content">
            <span>Derma Rolling</span> therapy is a salon procedure loved by
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
      <button class="our-product__btn"><img src="" alt="" /></button>
      <button class="our-product__btn"><img src="" alt="" /></button>
    </div>
  </div>
</template>

<script>
import TheLink from "./common/TheLink.vue";
export default {
    name: 'The-our-product',
    components: { TheLink },
};
</script>

<style lang="scss">
</style>

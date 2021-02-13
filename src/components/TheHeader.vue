<template>
  <div class="header">
    <a href="#" class="header__logo">
      <img src="../assets/Union.png" alt="" />
    </a>
    <div class="header__content">
        <h1 class="header__title">Do you love your skin? </h1>
        <span class="header__subtitle">PM loves your skin!</span>
        <div class="header__box">
            <the-button class="header__btn">Order now </the-button>
            <a href="/" class="header__link">Dermatologist consultation</a>
        </div>
    </div>
  </div>
</template>

<script>
import TheButton from './common/TheButton.vue';
export default {
    name: 'The-header',
    components: { TheButton },
};
</script>

<style lang="scss">
.header {
  min-height: 100vh;
  @include flex(center, center, column);
  position: relative;
  background-image: url('../assets/Render Passes.png');
  background-repeat:  no-repeat;
  background-color: $pink-color;
  width: 100%;
  &__logo{
      position: absolute;
      top: 57px;
      left: 50%;
      transform: translateX(-50%);
  }
  &__title{
      @include text($H1200, 900, $dark-color){
          max-width: 654px;
          text-align: left;
          line-height: 113px;
          letter-spacing: 1px;
          text-transform: capitalize;
      };
      margin-bottom: 12px;
  }
  &__subtitle{
      @include text($H240, 900, $dark-color){
          text-align: center;
          line-height: 27px;
          letter-spacing: 1px;
      };
      display: block;
      margin-bottom: 200px;
  }
  &__btn{
    margin-right: 50px;
  }
}
</style>

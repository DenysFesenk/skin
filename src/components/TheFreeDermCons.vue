<template>
  <div class="free-consultation">
    <h2 class="free-consultation__title">Free dermatologist consultation</h2>
    <div class="free-consultation__box">
      <div class="free-consultation__content">
        <p class="free-consultation__text free-consultation__text-first">
          We care about you, and we want to make your skin care experience truly
          professional and salon like.
        </p>
        <p class="free-consultation__text">
          We provide a free professional dermatologist consultation to every
          customer, because you are worth being beautiful every day!
        </p>
      </div>
      <form class="free-consultation__form">
        <input
          type="text"
          placeholder="Name"
          class="free-consultation__input"
        />
        <input
          type="text"
          placeholder="Email"
          class="free-consultation__input"
        />
        <input
          type="text"
          placeholder="№ sales check"
          class="free-consultation__input"
        />
        <textarea type="text" class="free-consultation__input" />
      </form>
    </div>
    <the-button>Send</the-button>
  </div>
</template>

<script>
import TheButton from "./common/TheButton.vue";

export default {
  components: { 
    TheButton,
   },
};
</script>

<style lang="scss">
.free-consultation {
    background-color: $grey-color;
    background-image: url('../assets/Vector.png');
    background-repeat: no-repeat;
    background-position: right 0;
    padding: 0 15% 195px;
    &__title{
        max-width: 692px;
        margin-bottom: 87px;
        @include text($H720, 900, $dark-color){
            line-height: 74px;
            letter-spacing: 2px;
            text-transform: capitalize;
        };
    }
  &__box {
      @include flex();
      margin-left: 39px;
      margin-bottom: 22px;
  }
  &__content{
      max-width: 540px;
      margin-right: 108px;
  }
  &__text{
      @include text($H240, 500, $black){
          opacity: .6;
          line-height: 39px;
          letter-spacing: .5px;
      };
  }
  &__text-first{
      font-weight: 700;
      margin-bottom: 21px;
  }
  &__form{
      @include flex(flex-start, stretch, column);
  }
  &__input{
      &:not(:last-child){
            margin-bottom: 20px; 
      };
      &:last-child{
          min-height: 80px;
      }
      background-color: $pink-btn;
      width: 270px;
      padding: 3.7px 6.3px 7px;
      outline: none;
      border: none;
      @include text($H80, 500, $grey-text){
        //   opacity: 0.53;
          line-height: 30px;
          letter-spacing: 0.5px;
      };
  }
  &__textarea{
      background-color: $pink-color;
      width: 270px;
      padding: 3.7px 6.3px 7px;
      outline: none;
      border: none;
      max-width: 270px;
  }
}
</style>

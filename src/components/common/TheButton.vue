<template>
  <button class="btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "The-button",
};
</script>

<style lang="scss">
.btn {
  @include text($H240, normal, $pink-color) {
    line-height: 28px;
    text-align: center;
    letter-spacing: 0.5px;
    text-transform: capitalize;
  }
  outline: none;
  border: none;
  cursor: pointer;
  position: relative;
  padding: 13px 32px;
  background-color: $dark-color;
  border-radius: 10px;
  @include transition;
  &:hover{
      background-color: $dark-link;
  }
  &:active{
      box-shadow: inset 0 0 15px 5px $dark-color;
  }
}
</style>

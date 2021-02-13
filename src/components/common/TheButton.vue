<template>
  <button class="btn">
      <slot></slot>
  </button>
</template>

<script>
export default {
    name: 'The-button',
}
</script>

<style lang="scss">
    .btn{
        background-image: url('../../assets/Union (1).png');
        @include text($H240, normal, $pink-color){
            line-height: 28px;
            text-align: center;
            letter-spacing: 0.5px;
            text-transform: capitalize;
        };
        outline: none;
        border: none;
        cursor: pointer;
    }
</style>
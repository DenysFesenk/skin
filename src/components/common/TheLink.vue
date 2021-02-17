<template>
  <a href="/" class="link">
    <span><slot></slot></span>
    <img src="../../assets/Arrow.png" alt="" />
  </a>
</template>

<script>
export default {
  name: "The-link",
};
</script>

<style lang="scss">
.link {
  text-decoration: none;
  span {
    margin-right: 12px;
    @include text($H80, 500, $dark-link) {
      line-height: 21px;
      letter-spacing: 0.5px;
    }
  }
}
</style>

<template>
  <div id="app">
      <the-header />
      <the-our-product />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheOurProduct from './components/TheOurProduct.vue'


export default {
  name: 'App',
  components: {
    TheHeader,
    TheOurProduct

  }
}
</script>

<style lang="scss">
#app {
  
}
</style>

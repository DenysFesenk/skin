<template>
  <div id="app">
      <the-header />
      <the-our-product />
      <the-free-derm-cons />
      <the-footer />
  </div>
</template>

<script>
import TheFooter from './components/TheFooter.vue'
import TheFreeDermCons from './components/TheFreeDermCons.vue'
import TheHeader from './components/TheHeader.vue'
import TheOurProduct from './components/TheOurProduct.vue'


export default {
  name: 'App',
  components: {
    TheHeader,
    TheOurProduct,
    TheFreeDermCons,
    TheFooter

  }
}
</script>

<style lang="scss">
#app {
  
}
</style>

<template>
  <div id="app">
    
    <Header/>

    <Products/>

    <Footer/> 

  </div>
</template>

<script>
import Header from './components/Header.vue';
// import Products from './components/Products.vue';
// import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    // Products,
    // Footer

  }
}
</script>

<style lang="scss">
@import 'style/commons.scss';

</style>

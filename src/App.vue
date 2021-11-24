<template>
  <div>
    <Header />
    <Main />
    <MenuShop />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import MenuShop from './components/MenuShop.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    MenuShop,
    Footer  
  }
}
</script>

<style lang="scss">
  @import "./assets/style/vars.scss";
  @import "./assets/style/general.scss";
</style>

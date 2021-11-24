<template>
  <header class="container">

    <div class="header__left">
      <a href="#"><img src="../assets/img/dc-logo.png" alt="Logo Dc"></a>
    </div>
    
      <div class="header__right">
        <MenuNav />
      </div>

  </header> 
</template>

<script>
import MenuNav from './MenuNav.vue'

export default {
  name: 'Header',
  components: {
    MenuNav  
  }
}

</script>

<style lang="scss" scoped>
@import "../assets/style/mixins.scss";

header {
  display: flex;
  justify-content: space-between;
  line-height: 100px
}

.header__left {
  
  img {
    width: 75px;
    vertical-align: middle
  }
}

</style>
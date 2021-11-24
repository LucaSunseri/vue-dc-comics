<template>
  <div>
    <div class="container">

      <div v-for="(box, index) in boxsShop" :Key="index" class="box">
        <img :src="require(`../assets/img/${box.logo}`)" :alt="box.name">
        <span>{{box.name}}</span>
      </div>

    </div>
  </div> 
</template>

<script>
export default {
  name: 'MenuShop',
  data() {
    return {
      boxsShop: [
      {
        name: 'DIGITAL COMICS',
        logo: 'buy-comics-digital-comics.png',
      },
      {
        name: 'DC MERCHANDISE',
        logo: 'buy-comics-merchandise.png',
      },
      {
        name: 'PRINT SUBSCRIPTIONS',
        logo: 'buy-comics-subscriptions.png',
      },
      {
        name: 'COMIC SHOP LOCATOR',
        logo: 'buy-comics-shop-locator.png',
      },
      {
        name: 'DC POWER VISA',
        logo: 'buy-dc-power-visa.svg',
      },
    ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";

div {
  background-color: $primary-color;
  color: #fff;
  padding: 10px 0;
  .container {
    display: flex;
    .box {
      @include center;
      flex-basis: calc(100% / 5);
      padding: 20 15px;
      cursor: pointer;
      img {
        width: 35px;
        margin-right: 10px;
      }
      span {
        font-size: 12px;
      }
    }
  }
}

</style>
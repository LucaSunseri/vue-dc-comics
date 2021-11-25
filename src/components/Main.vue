<template>
  <main>
    <div class="container">

      <div class="title">
        <h2>CURRENT SERIES</h2>
      </div>

      <div class="series">
        <div v-for="(card, index) in contentCards" :key="index" class="series__box">
          <Card :contentCard="card" />
        </div>
      </div>

      <div class="button">
        <span>LOAD MORE</span>
      </div>

    </div>
  </main> 
</template>

<script>
import Card from './Card.vue';
import contentCards from '../assets/data/ArrayCardMain.js'

export default {
  name: 'Main',
  components: {
    Card 
  },
  data() {
    return {
      contentCards
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

main {
  background-color: rgba(0, 0, 0, 0.836);
  .title {
    position: relative;
    z-index: 100;
    margin-top: -25px;
    h2 {
      display: inline-block;
      background-color: $primary-color;
      font-weight: 900;
      padding: 10px 20px;
      color: #fff;
    }
  }

  .series {
    display: flex;
    flex-wrap: wrap;
    margin-top: 30px;
    padding: 50px 10px;
  }

  .series__box {
    display: flex;
    justify-content: center;
    flex-basis: calc(100% / 6);
    padding: 10px 0;
  }

}

</style>
<template>
  <div class="card">
    <div class="card__img">
      <img :src="contentCard.thumb" :alt="contentCard.series">
    </div>
    <div class="card__text">
      <p>{{contentCard.series}}</p>
    </div>
  </div> 
</template>

<script>
export default {
  name: 'Card',
  props: {
    contentCard: Object,
  }
}
</script>

<style lang="scss" scoped>

.card {
  width: 150px;
  display: flex;
  flex-direction: column;
}

.card__img {
  width: 100%;
  height: 150px;
  overflow: hidden;
  img {
    width: 100%;
  }
}

.card__text {
  margin-top: 10px;
  p {
    text-transform: uppercase;
    color: #fff;
    font-size: 12px;
  }
}

</style>
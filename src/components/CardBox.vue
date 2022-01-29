<template>
  <div class="box-card">
    <div class="container-card">
      <div v-for="(card, index) in cards" :key="index" class="card">
        <div class="content-image">
          <img :src="card.thumb" alt="" />
        </div>
        <p>{{ card.series.toUpperCase() }}</p>
        <p>PRICE: {{ card.price }}</p>
      </div>
    </div>

    <div class="other-series">
      <a href="#">LOAD MORE</a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    cards: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/cardApp.scss";
</style>
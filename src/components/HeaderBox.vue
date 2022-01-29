<template>
  <header>
    <div class="container">
      <div class="content-logo">
        <img src="../assets/dc-logo.png" alt="" />
      </div>

      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">{{ link }}</li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  props: {
    links: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/headerApp.scss";
</style>
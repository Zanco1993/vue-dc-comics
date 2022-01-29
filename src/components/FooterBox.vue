<template>
  <footer>
    <footer-info />
    <footer-link />
    <footer-social />
  </footer>
</template>

<script>
import FooterInfo from "../components/FooterInfo.vue";
import FooterLink from "../components/FooterLink.vue";
import FooterSocial from "../components/FooterSocial.vue";

export default {
  components: {
    FooterInfo,
    FooterLink,
    FooterSocial,
  },
};
</script>

<style lang="scss" scoped>
</style>
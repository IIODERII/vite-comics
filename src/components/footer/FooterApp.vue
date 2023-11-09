<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterBottom from "./FooterBottom.vue";
export default {
  name: "FooterApp",
  components: {
    FooterTop,
    FooterBottom,
  },
};
</script>

<style lang="scss" scoped>
footer {
  margin-top: -20px;
}
</style>

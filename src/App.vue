<template>
  <HeaderApp />
  <MainApp />
  <FooterApp />
</template>

<script>
import HeaderApp from "./components/header/HeaderApp.vue";
import MainApp from "./components/main/MainApp.vue";
import FooterApp from "./components/footer/FooterApp.vue";

export default {
  name: "App",
  components: {
    HeaderApp,
    MainApp,
    FooterApp,
  },
  mounted() {
    console.log(comics);
  },
};
</script>

<style lang="scss" scoped></style>

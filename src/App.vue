<template>
  <HeaderApp />
  <MainApp />
  <FooterApp />
</template>

<script>
import HeaderApp from "./components/header/headerapp.vue";
import MainApp from "./components/main/mainapp.vue";
import FooterApp from "./components/footer/FooterApp.vue";
export default {
  name: "App",
  components: {
    HeaderApp,
    MainApp,
    FooterApp,
  },
};
</script>

<style lang="scss" scoped></style>

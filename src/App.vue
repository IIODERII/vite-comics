<template>
  <HeaderApp />
  <MainApp />
</template>

<script>
import HeaderApp from "./components/header/HeaderApp.vue";
import MainApp from "./components/main/MainApp.vue";
export default {
  name: "App",
  components: {
    HeaderApp,
    MainApp,
  },
};
</script>

<style lang="scss" scoped></style>

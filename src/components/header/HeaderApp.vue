<template>
  <header class="bg-white">
    <div
      class="container d-flex flex-lg-nowrap flex-wrap justify-content-between align-items-center"
    >
      <div class="mx-auto">
        <img src="../../assets/image/dc-logo.png" alt="Small Logo" />
      </div>

      <NavApp class="flex-lg-nowrap justify-content-center" />
    </div>
  </header>
</template>

<script>
import NavApp from "./NavApp.vue";
export default {
  name: "HeaderApp",
  components: {
    NavApp,
  },
};
</script>

<style lang="scss" scoped></style>

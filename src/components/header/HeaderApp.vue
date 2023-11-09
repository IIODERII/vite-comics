<template>
  <header class="bg-white py-3">
    <div class="container d-flex justify-content-between align-items-center">
      <div>
        <img src="../../assets/image/dc-logo.png" alt="Small Logo" />
      </div>

      <NavApp />
    </div>
  </header>
</template>

<script>
import NavApp from "./navapp.vue";
export default {
  name: "HeaderApp",
  components: {
    NavApp,
  },
};
</script>

<style lang="scss" scoped></style>

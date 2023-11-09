<template>
  <main>
    <MainTop />
    <MainBottom />
  </main>
</template>

<script>
import MainTop from "./MainTop.vue";
import MainBottom from "./MainBottom.vue";
export default {
  name: "MainApp",
  components: { MainTop, MainBottom },
};
</script>

<style lang="scss" scoped></style>

<template>
  <div class="jumbo position-relative">
    <div class="container">
      <button class="btn btn-primary rounded-0">Current series</button>
    </div>
  </div>

  <div class="bg-black text-white">
    <div class="container fs-3 fw-bold py-5">
      <Comics />
    </div>
  </div>
</template>

<script>
import Comics from "./Comics.vue";
export default {
  name: "MainTop",
  components: {
    Comics,
  },
};
</script>

<style lang="scss" scoped>
.jumbo {
  height: 500px;
  background-image: url("../../assets/image/jumbotron.jpg");
  background-position: center top;
  background-repeat: no-repeat;
  background-size: cover;

  button {
    position: absolute;
    top: 96%;
  }
}
</style>

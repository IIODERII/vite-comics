<template>
  <div class="row align-items-start">
    <ComicCard
      v-for="comic in comics"
      :image="comic.thumb"
      :title="comic.series"
      :cost="comic.price"
    />
  </div>
</template>

<script>
import { comics } from "../../assets/data.js";
import ComicCard from "./ComicCard.vue";

export default {
  name: "Comics",
  components: {
    ComicCard,
  },
  data() {
    return {
      comics: comics,
    };
  },
};
</script>

<style lang="scss" scoped></style>

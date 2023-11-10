<template>
  <div class="text-white col-12 col-md-6 col-lg-4 col-xxl-3 py-2">
    <div class="c-img">
      <img :src="image" :alt="title" />
    </div>
    <div class="py-2">
      <h5>{{ title }}</h5>
      <span>{{ cost }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "ComicCard",
  props: {
    image: String,
    title: String,
    cost: String,
  },
};
</script>

<style lang="scss" scoped>
.text-white {
  > div {
    margin: 0 auto;
    max-width: 300px;
  }
  &:hover {
    cursor: pointer;
    transform: scale(1.05);
    transition: all 0.3s ease;

    > div {
      color: #0d6efd;
      transition: all 0.2s ease;
    }
  }
  .c-img {
    height: 300px;
    width: 300px;
    img {
      height: 100%;
      width: 100%;
      object-fit: cover;
      object-position: center top;
    }
  }
}

@media screen and (max-width: 768px) {
  .text-white {
    .c-img {
      width: 100%;
      height: 85vw;
    }
  }
}
</style>

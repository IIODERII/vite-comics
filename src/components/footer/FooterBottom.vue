<template>
  <div class="my-bg">
    <div
      class="container py-5 d-flex justify-content-between align-items-center"
    >
      <div>
        <button
          class="text-uppercase btn btn-outline-primary border-3 text-white fw-bold rounded-0"
        >
          sign-up now
        </button>
      </div>

      <div class="d-flex flex-wrap justify-content-end">
        <h3 class="text-primary text-uppercase px-3 fw-bold py-2 text-end">
          follow us
        </h3>
        <ul class="d-flex flex-wrap justify-content-center list-unstyled">
          <li v-for="item in links" class="p-2">
            <img :src="item" :alt="item" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterBottom",
  data() {
    return {
      links: [
        "/img/footer/footer-facebook.png",
        "/img/footer/footer-twitter.png",
        "/img/footer/footer-youtube.png",
        "/img/footer/footer-pinterest.png",
        "/img/footer/footer-periscope.png",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.my-bg {
  background-color: #303030;

  img:hover {
    cursor: pointer;
    filter: invert(1);
    transition: all 0.3s ease-in-out;
  }

  @media screen and (max-width: 576px) {
    h3 {
      width: 100%;
    }
  }
}
</style>

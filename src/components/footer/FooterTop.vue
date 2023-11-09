<template>
  <div class="wrapper text-white">
    <div class="container d-flex justify-content-between align-items-center">
      <div class="row g-2 w-50">
        <div class="col-4">
          <h3 class="text-uppercase fw-bold">dc comics</h3>
          <ul class="list-unstyled">
            <li v-for="item in dcComics">
              <a href="#" class="text-decoration-none">{{ item }}</a>
            </li>
          </ul>

          <h3 class="text-uppercase fw-bold">Shop</h3>
          <ul class="list-unstyled">
            <li v-for="item in shop">
              <a href="#" class="text-decoration-none">{{ item }}</a>
            </li>
          </ul>
        </div>

        <div class="col-4">
          <h3 class="text-uppercase fw-bold">dc</h3>
          <ul class="list-unstyled">
            <li v-for="item in DC">
              <a href="#" class="text-decoration-none">{{ item }}</a>
            </li>
          </ul>
        </div>

        <div class="col-4">
          <h3 class="text-uppercase fw-bold">sites</h3>
          <ul class="list-unstyled">
            <li v-for="item in sites">
              <a href="#" class="text-decoration-none">{{ item }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="image">
        <img src="../../assets/image/dc-logo-bg.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
  data() {
    return {
      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],

      shop: ["Shop DC", "Shop DC Collectibles"],

      DC: [
        "Terms Of Use",
        "Privacy Policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],

      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
    };
  },
};
</script>

<style lang="scss" scoped>
.wrapper {
  background-image: url("../../assets/image/footer-bg.jpg");
  background-size: cover;
  overflow: hidden;
  height: 580px;

  h3 {
    font-size: 1.3em;
  }

  a {
    color: #999;
    font-size: 0.8em;

    &:hover {
      text-decoration: underline !important;
      color: #0d6efd;
    }
  }

  .image {
    width: 50%;
    img {
      width: 100%;
      transform: translateY(-5%);
    }
  }
}
</style>

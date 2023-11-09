<template>
  <div class="bg-primary">
    <div class="container">
      <ul
        class="d-flex list-unstyled justify-content-between text-uppercase text-white"
      >
        <li
          v-for="item in buyList"
          class="d-flex align-items-center justify-content-between py-5"
        >
          <div>
            <img :src="item.image" :alt="item.text" class="h-100" />
          </div>
          {{ item.text }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainBottom",
  data() {
    return {
      buyList: [
        {
          text: "Digital Comics",
          image: "/img/buy/buy-comics-digital-comics.png",
        },
        {
          text: "DC Merchandise",
          image: "/img/buy/buy-comics-merchandise.png",
        },
        {
          text: "Subscription",
          image: "/img/buy/buy-comics-subscriptions.png",
        },
        {
          text: "Comic shop locator",
          image: "/img/buy/buy-comics-shop-locator.png",
        },
        {
          text: "DC power visa",
          image: "/img/buy/buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
ul {
  li {
    div {
      height: 80px;
      padding: 0 20px;
    }
    &:hover {
      cursor: pointer;
      background-color: rgba(255, 255, 255, 0.1);
      transition: all 0.3s ease;
    }
  }
  & li:last-child div {
    height: 60px;
  }
}
</style>

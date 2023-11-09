<template>
  <ul class="nav nav-underline text-uppercase">
    <li class="nav-item px-1" v-for="(item, index) in navItems">
      <a
        class="nav-link py-5 text-black fw-bold"
        :class="{ active: item.active }"
        aria-current="page"
        :href="item.url"
        @click="changePage(index)"
        >{{ item.text }}</a
      >
    </li>
  </ul>
</template>

<script>
export default {
  name: "NavApp",
  data() {
    return {
      navItems: [
        {
          text: "Characters",
          active: false,
          url: "#",
        },
        {
          text: "Comics",
          active: true,
          url: "#",
        },
        {
          text: "Movies",
          active: false,
          url: "#",
        },
        {
          text: "Tv",
          active: false,
          url: "#",
        },
        {
          text: "Games",
          active: false,
          url: "#",
        },
        {
          text: "Collectibles",
          active: false,
          url: "#",
        },
        {
          text: "Videos",
          active: false,
          url: "#",
        },
        {
          text: "Fans",
          active: false,
          url: "#",
        },
        {
          text: "News",
          active: false,
          url: "#",
        },
        {
          text: "Shop",
          active: false,
          url: "#",
        },
      ],
    };
  },
  methods: {
    changePage(i) {
      this.navItems.forEach((item) => {
        item.active = false;
      });
      this.navItems[i].active = true;
    },
  },
};
</script>

<style lang="scss" scoped>
.active {
  color: #0c7cec !important;
}

a {
  font-size: 0.9em;
}
</style>

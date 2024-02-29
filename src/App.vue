<template>
  <header class="nav-bar">
    <div>
      <MainHeader />
    </div>
  </header>
  <body>
    <HomePage />
  </body>

  <!-- <RouterView /> -->
</template>

<script>
import { RouterLink, RouterView } from "vue-router";
import HomePage from "./views/HomePage.vue";
import MainHeader from "./components/MainHeader.vue";

export default {
  components: {
    HomePage,
    MainHeader,
  },
  methods: {
    stickyNav() {
      const primaryHeader = document.querySelector(".nav-bar");
      const scrollWatcher = document.createElement("div");

      scrollWatcher.setAttribute("data-scroll-watcher", "");
      primaryHeader.before(scrollWatcher);

      const navObserver = new IntersectionObserver(
        (entries) => {
          primaryHeader.classList.toggle(
            "sticking",
            !entries[0].isIntersecting
          );
        },
        { rootMargin: "300px 0px 0px 0px" }
      );
      navObserver.observe(scrollWatcher);
    },
  },
  mounted() {
    this.stickyNav();
  },
};
</script>

<script></script>

<style scoped>
.nav-bar.sticking {
  position: sticky;
  top: 0;
  z-index: 10;
}

.nav-bar.sticking .header-area {
  background-color: #fff;
  box-shadow: 0 10px 5px rgba(0, 0, 0, 0.1);
  transition: all 300ms ease;
}
</style>

<template>
  <header>
    <MainHeader />
  </header>
  <body>
    <HomePage />
  </body>

  <!-- <RouterView /> -->
</template>

<script setup>
import { RouterLink, RouterView } from "vue-router";
import HomePage from "./views/HomePage.vue";
import MainHeader from "./components/MainHeader.vue";
</script>

<style scoped></style>

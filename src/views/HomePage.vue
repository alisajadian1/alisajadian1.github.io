<template>
  <main>
    <HeroSection />
    <AboutSection />
  </main>
</template>

<script>
import HeroSection from "@/components/HeroSection.vue";
import AboutSection from "@/components/AboutSection.vue";
export default {
  components: {
    HeroSection,
    AboutSection,
  },
};
</script>

<template>
  <main>
    <HeroSection />
    <AboutSection />
    <ResumeSection />
  </main>
</template>

<script>
import HeroSection from "@/components/HeroSection.vue";
import AboutSection from "@/components/AboutSection.vue";
import ResumeSection from "@/components/ResumeSection.vue";

export default {
  components: {
    HeroSection,
    AboutSection,
    ResumeSection,
  },
};
</script>

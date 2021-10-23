<template>
  <main class="home">
    <Hero />
    <About />
    <News />
    <Cta />
  </main>
</template>

<script>
import Hero from "@/components/Hero.vue";
import About from "@/components/About.vue";
import News from "@/components/News.vue";
import Cta from "@/components/Cta.vue";

export default {
  name: "Home",
  components: { Hero, About, News, Cta },
};
</script>

<style lang="scss" scoped>
.home {
  overflow: hidden;
}
</style>

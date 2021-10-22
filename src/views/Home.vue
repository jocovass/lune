<template>
  <main class="home">
    <Hero />
    <About />
    <News />
  </main>
</template>

<script>
import Hero from "@/components/Hero.vue";
import About from "@/components/About.vue";
import News from "@/components/News.vue";

export default {
  name: "Home",
  components: { Hero, About, News },
};
</script>

<style lang="scss" scoped>
.home {
  overflow: hidden;
}
</style>

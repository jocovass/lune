<template>
  <header class="header">
    <div class="content">
      <img alt="Vue logo" src="../assets/logo-sm.svg" width="65" />
      <Navigation />
    </div>
  </header>
</template>

<script>
import Navigation from "@/components/Navigation.vue";
export default {
  components: { Navigation },
};
</script>

<style lang="scss" scoped>
.header {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 10;
}
.header .content {
  padding: 1rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>

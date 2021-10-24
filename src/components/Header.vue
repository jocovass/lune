<template>
  <header class="header">
    <div class="content">
      <img alt="Vue logo" src="../assets/logo-sm.svg" width="65" />
      <MobileNav v-if="isMobile" />
      <DesktopNav v-else />
    </div>
  </header>
</template>

<script>
import DesktopNav from "@/components/DesktopNav.vue";
import MobileNav from "@/components/MobileNav.vue";
export default {
  components: { DesktopNav, MobileNav },
  data() {
    return {
      isMobile: false,
    };
  },
  created() {
    this.checkDeviceSize();
    window.addEventListener("resize", this.checkDeviceSize);
  },
  beforeDestroy() {
    window.removeEventListener("resize", this.checkDeviceSize);
  },
  methods: {
    checkDeviceSize() {
      window.matchMedia("(min-width: 768px").matches
        ? (this.isMobile = false)
        : (this.isMobile = true);
    },
  },
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

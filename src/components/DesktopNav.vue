<template>
  <nav class="nav">
    <NavigationList />
  </nav>
</template>

<script>
import NavigationList from "@/components/NavigationList.vue";

export default {
  components: {
    NavigationList,
  },
};
</script>

<style lang="scss" scoped>
.nav {
  &__list {
    display: flex;
    align-items: center;
  }
}
</style>

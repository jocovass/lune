<template>
  <div class="mobile-navigation">
    <button class="hamburger-btn" @click="toggleNavigation">
      <Icon icon="bars" />
    </button>
    <transition name="slide-in" @after-enter="openNavlist = true">
      <div v-show="isNavigationOpen" class="nav__container">
        <transition name="grow" @after-leave="isNavigationOpen = false">
          <nav v-show="openNavlist" class="nav">
            <NavigationList />
          </nav>
        </transition>
      </div>
    </transition>
  </div>
</template>

<script>
import NavigationList from "@/components/NavigationList.vue";

export default {
  components: { NavigationList },
  data() {
    return {
      isNavigationOpen: true,
      openNavlist: true,
    };
  },
  methods: {
    toggleNavigation() {
      if (this.isNavigationOpen) {
        this.openNavlist = false;
      } else {
        this.isNavigationOpen = true;
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.mobile-navigation {
  position: relative;
}
.hamburger-btn {
  position: relative;
  z-index: 50;
  background-color: transparent;
  border: none;
  outline: none;
  cursor: pointer;
  svg {
    color: $white;
    width: 1.5rem;
    height: 1.5rem;
  }
}

.nav__container {
  position: fixed;
  z-index: 40;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.nav {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: $black;
  text-align: center;

  &__item {
    margin-bottom: 1rem;
    padding: 2rem;
  }

  &__link {
    padding: 2rem;
    color: green;
  }
}

.grow-enter-active {
  transition: clip-path 0.3s ease-out;
  clip-path: circle(0% at 99% 1%);
}

.grow-leave-active {
  transition: clip-path 0.3s ease-out;
  clip-path: circle(75%);
}

.grow-enter-to {
  clip-path: circle(75%);
}
.grow-leave-to {
  clip-path: circle(0% at 99% 1%);
}

.slide-in-enter-active {
  transform: translateX(100%);
}

.slide-in-enter-to {
  transform: translateX(0%);
}
.slide-in-leave-to {
  transform: translateX(100%);
}
</style>

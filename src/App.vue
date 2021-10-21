<template>
  <div id="app">
    <Header />
    <router-view />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
  name: "App",
  components: { Header },
};
</script>

<style lang="scss">
*,
*::before,
*::after {
  box-sizing: inherit;
  padding: 0;
  margin: 0;
}

body {
  box-sizing: border-box;
  font-family: "Merriweather", serif;
  background-color: $black;
  color: $white;
}

ul {
  list-style: none;
}

.content {
  width: 95%;
  max-width: 1350px;
  margin: 0 auto;
}

.btn {
  text-decoration: none;
  display: inline-block;
}

.btn-primary {
  background-color: $pink;
  color: $white;
  padding: 0.35em 1em;
  border-radius: 100px;
  transition: background 0.35s ease-out;

  &:hover,
  &:focus,
  &:active {
    background-color: $green;
  }
}

.btn-secondary {
  background-color: $green;
  color: $light-blue;
  padding: 0.8em 1.2em;
  border-radius: 10px;
  transition: background 0.35s ease-out;
  font-weight: bold;

  &:hover,
  &:focus,
  &:active {
    background-color: $pink;
  }
}
</style>

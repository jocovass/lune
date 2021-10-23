<template>
  <div id="app">
    <Header />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "App",
  components: { Header, Footer },
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

p {
  font-weight: 300;
  letter-spacing: 0.6px;
  line-height: 1.4;
}

h2 {
  font-size: 2.5rem;
  margin-bottom: 0.8rem;
}

.content {
  width: 95%;
  max-width: 1350px;
  margin: 0 auto;
}

.text-box {
  max-width: 800px;
  text-align: center;
  margin: 0 auto;
}

.btn {
  text-decoration: none;
  display: inline-block;
  border: none;
  font-family: inherit;
  cursor: pointer;
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

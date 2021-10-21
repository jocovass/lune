<template>
  <nav class="nav">
    <ul class="nav__list">
      <li class="nav__item"><a href="/home" class="nav__link">Home</a></li>
      <li class="nav__item">
        <a href="/my-watchlist" class="nav__link">My WatchList</a>
      </li>
      <li class="nav__item"><a href="/stock" class="nav__link">Stocks</a></li>
      <li class="nav__item"><a href="/login" class="nav__link">Login</a></li>
      <li class="nav__item">
        <a href="/sign-up" class="btn btn-primary">Sing up</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss">
.nav {
  &__list {
    display: flex;
    align-items: center;
  }
  &__item:not(:last-of-type) {
    margin-right: 1.5rem;
  }

  &__link {
    color: $white;
    text-decoration: none;
    transition: color 0.15s ease-out;

    &:hover,
    &:focus,
    &:active {
      color: $pink;
    }
  }
}
</style>

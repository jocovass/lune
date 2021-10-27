<template>
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
</template>

<script>
export default {};
</script>

<style lang="scss">
.nav {
  &__item {
    margin-bottom: 1rem;
  }

  .btn {
    margin-top: 2rem;
  }

  &__link {
    display: inline-block;
    padding: 0.2em;
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

@media only screen and (min-width: "768px") {
  .nav {
    &__item {
      margin-bottom: 0;
      margin-right: 1rem;
    }

    .btn {
      margin-top: 0;
      margin-left: 2rem;
    }
  }
}
</style>

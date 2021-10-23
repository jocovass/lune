<template>
  <div class="social">
    <ul class="social__links">
      <li class="social__item">
        <a target="_blank" href="https://twitter.com" class="social__link">
          <Icon :icon="['fab', 'twitter']" />
        </a>
      </li>
      <li class="social__item">
        <a target="_blank" href="https://facebook.com" class="social__link">
          <Icon :icon="['fab', 'facebook']" />
        </a>
      </li>
      <li class="social__item">
        <a target="_blank" href="https://linkedin.com" class="social__link">
          <Icon :icon="['fab', 'linkedin']" />
        </a>
      </li>
      <li class="social__item">
        <a target="_blank" href="https://instagram.com" class="social__link">
          <Icon :icon="['fab', 'instagram']" />
        </a>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.social {
  &__links {
    display: flex;
  }

  &__item {
    margin-right: 1.1rem;
  }

  &__link {
    color: $white;
    transition: color 0.15s ease-out;

    svg {
      width: 1.5rem;
      height: 1.5rem;
    }

    &:hover,
    &:focus,
    &:active {
      color: $pink;
    }
  }
}
</style>

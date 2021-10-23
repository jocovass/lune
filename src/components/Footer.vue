<template>
  <footer class="footer">
    <div class="content">
      <div class="col-1-4">
        <div class="logo">
          <img
            src="@/assets/logo-sm.svg"
            alt="Lune logo"
            width="45"
            height="45"
          />
          <span>Lune</span>
        </div>
        <SocialLinks />
      </div>
      <div class="col-1-4">
        <ul class="footer-nav__list">
          <li class="footer-nav__item">
            <a href="/stocks" class="footer-nav__link">Stocks</a>
          </li>
          <li class="footer-nav__item">
            <a href="/my-watchlist" class="footer-nav__link">My Watchlist</a>
          </li>
          <li class="footer-nav__item">
            <a href="/news" class="footer-nav__link">Latest News</a>
          </li>
        </ul>
      </div>
      <div class="col-1-2">
        <NewsletterSubscription />
      </div>
    </div>
  </footer>
</template>

<script>
import SocialLinks from "@/components/SocialLinks.vue";
import NewsletterSubscription from "@/components/NewsletterSubscription.vue";

export default {
  components: {
    SocialLinks,
    NewsletterSubscription,
  },
};
</script>

<style lang="scss" scoped>
.footer {
  padding: $section-padding 0;
  .content {
    display: flex;
    justify-content: space-between;
  }
}

.logo {
  margin-bottom: 1rem;
  display: flex;

  span {
    display: block;
    font-size: 1.3rem;
    font-weight: 700;
    font-style: italic;
    margin-left: 5px;
    margin-bottom: 2px;
    margin-top: auto;
  }
}

.footer-nav {
  &__link {
    color: $white;
    text-decoration: none;
    display: inline-block;
    padding: 0.1em 0.3em;
    margin-bottom: 0.3em;
    transition: color 0.15s ease-out;

    &:hover,
    &:focus,
    &:active {
      color: $pink;
    }
  }
}
</style>

<template>
  <section class="cta">
    <div class="content">
      <div class="text-box">
        <h2>Sign up today and discover the power over financial freedom</h2>
        <a href="/sign-up" class="btn btn-secondary">Sign up</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.cta {
  background-color: $light-black;
  padding: $section-padding 0;

  .text-box {
    max-width: 400px;
  }
}

.btn {
  margin-top: 1.4rem;
}

@media only screen and (min-width: "768px") {
  .cta {
    padding: calc(#{$section-padding * 2}) 0;

    .text-box {
      width: 70%;
      max-width: 800px;
    }
  }
}
</style>

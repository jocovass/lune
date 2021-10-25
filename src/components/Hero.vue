<template>
  <section class="hero">
    <div class="content">
      <img src="@/assets/images/hero.svg" alt="" width="650" />

      <div class="col-1">
        <h1>Start Building Your Wealth</h1>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusamus
          rem commodi suscipit eveniet omnis nihil, quam obcaecati optio,
          consequuntur alias minus quasi, nam porro nemo facilis officia
          incidunt corrupti excepturi?
        </p>
        <a href="/sign-up" class="btn btn-secondary">Get Started</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  // height: 80vh;
  // min-height: 600px;
  // display: flex;
  // align-items: center;

  .content {
    // display: flex;
    position: relative;
  }

  .col-1 {
    // flex-basis: 45%;
    padding-top: 17rem;
    padding-bottom: 1.2rem;
  }

  .btn {
    margin: 1.5rem 0;
  }

  img {
    width: 400px;
    position: absolute;
    top: 0;
    left: 0;
    transform: translate(-12%, -40%);
    // top: 50%;
    // left: 50%;
    // transform: translateY(-45%);
  }
}
</style>

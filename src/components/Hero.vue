<template>
  <section class="hero">
    <div class="content">
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
      <img
        src="@/assets/images/hero.svg"
        alt=""
        width="650"
        style="position: absolute"
      />
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  height: 80vh;
  min-height: 600px;
  display: flex;
  align-items: center;

  .content {
    display: flex;
    position: relative;
  }

  .col-1 {
    flex-basis: 45%;
  }

  h1 {
    font-size: 3.2rem;
    margin-bottom: 0.8rem;
  }

  .btn {
    margin: 1.5rem 0;
  }

  img {
    width: 950px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-45%);
  }
}
</style>

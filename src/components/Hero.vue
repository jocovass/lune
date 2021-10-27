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
  .content {
    position: relative;
  }

  .col-1 {
    padding-top: 17rem;
    padding-bottom: 1.2rem;
    max-width: 400px;
    margin: 0 auto;
  }

  .btn {
    margin: 1.5rem 0;
  }

  img {
    width: 90%;
    min-width: 400px;
    max-width: 550px;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translate(-50%, -40%);
  }
}

@media only screen and (min-width: "500px") {
  .hero {
    .col-1 {
      padding-top: calc(58vw * 0.9);
    }
  }
}

@media only screen and (min-width: "768px") {
  .hero {
    height: 80vh;
    min-height: 600px;
    display: flex;
    align-items: center;

    .content {
      display: flex;
    }

    .col-1 {
      max-width: initial;
      margin: 0;
      padding-top: 0;
      flex-basis: 45%;
    }

    img {
      max-width: 700px;
      top: 50%;
      left: 50%;
      transform: translate(0%, -50%);
    }
  }
}

@media only screen and (min-width: "1200px") {
  .hero {
    img {
      max-width: 800px;
    }
  }
}
</style>

<template>
  <section class="about">
    <div class="content">
      <div class="image-container">
        <img
          src="@/assets/images/versatile.svg"
          alt="Mobile phone with trading options popping up"
        />
      </div>
      <div class="col-1-2">
        <h2>Why choose Lune?</h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusamus
          rem commodi suscipit eveniet omnis nihil, quam obcaecati optio,
          consequuntur alias minus quasi, nam porro nemo facilis officia
          incidunt corrupti excepturi?
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.about {
  background-color: $light-black;
  padding: $section-padding 0;

  .col-1-2 {
    max-width: 400px;
    margin: 0 auto;
  }

  .image-container {
    text-align: center;
    margin-bottom: 2.5rem;
  }

  img {
    width: 100%;
    max-width: 280px;
  }
}

@media only screen and (min-width: "768px") {
  .about {
    padding: calc(#{$section-padding} * 2) 0;

    .content {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .col-1-2 {
      flex-basis: 48%;
      max-width: initial;
      margin: 0;
    }

    .image-container {
      margin-bottom: 0;
      flex-basis: 47%;
    }

    img {
      max-width: 500px;
    }
  }
}

@media only screen and (min-width: "1200px") {
  .about {
    .col-1-2 {
      flex-basis: 45%;
    }
  }
}
</style>

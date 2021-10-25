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
  // padding: calc(#{$section-padding} * 2) 0;
  padding: $section-padding 0;

  .content {
    // display: flex;
    // align-items: center;
    // justify-content: space-between;
  }

  .col-1-2 {
    // width: 45%;
  }

  .image-container {
    text-align: center;
    margin-bottom: 2rem;
  }

  img {
    width: 280px;
  }
}
</style>

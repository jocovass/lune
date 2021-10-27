<template>
  <section class="news">
    <div class="content">
      <div class="text-box">
        <h2>Do you like to stay up to date with the latest news?</h2>
        <p>
          It was popularised in the 1960s with the release of Letraset sheets
          containing Lorem Ipsum passages, and more recently with desktop
          publishing software like Aldus PageMaker including versions of Lorem
          Ipsum.
        </p>
      </div>
      <img src="@/assets/images/map.svg" alt="World map mockup with dots" />
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.news {
  padding: $section-padding 0;

  .text-box {
    margin-bottom: 3rem;
    max-width: 400px;
  }

  img {
    width: 100%;
    max-width: 1250px;
    margin: 0 auto;
    display: block;
  }
}

@media only screen and (min-width: "768px") {
  .news {
    padding: calc(#{$section-padding} * 2) 0;

    .text-box {
      margin-bottom: 5rem;
      width: 70%;
      max-width: 800px;
    }
  }
}

@media only screen and (min-width: "1200px") {
  .news {
    .text-box {
      margin-bottom: 7rem;
    }
  }
}
</style>

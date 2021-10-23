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
  padding: calc(#{$section-padding} * 2) 0;
}

.text-box {
  margin-bottom: 5rem;
}

img {
  width: 100%;
}
</style>

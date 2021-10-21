<template>
  <div class="hero">
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
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  height: 80vh;
  min-height: 600px;
  background-color: rgba(orangered, 0.4);
  display: flex;
  align-items: center;
  overflow-x: hidden;

  .content {
    display: flex;
    position: relative;
  }

  .col-1 {
    flex-basis: 45%;
  }

  h1 {
    font-size: 3.2rem;
  }

  p {
    font-weight: 300;
    letter-spacing: 0.6px;
    line-height: 1.4;
  }

  .btn {
    margin: 1.5rem 0;
  }

  img {
    width: 950px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%);
  }
}
</style>

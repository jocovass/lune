<template>
  <div class="newsletter">
    <h4>Get notified with the latest news</h4>
    <form class="newsletter-form">
      <div class="form-field">
        <label class="form-label" for="email">Email Address</label>
        <input
          id="email"
          name="email"
          class="form-input"
          placeholder="Email address"
          type="email"
        />
      </div>
      <button class="btn btn-primary" type="submit">Get Notified</button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.newsletter {
  margin-left: auto;
  &-form {
    display: flex;
  }
  h4 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
  }

  .btn {
    font-size: 1rem;
  }

  .form-field {
    margin-right: 0.7rem;
  }
}

.form-label {
  display: none;
}
.form-input {
  font-size: 1rem;
  font-family: inherit;
  font-weight: 300;
  padding: 0.4em 1.4em;
  border-radius: 100px;
  color: rgba($white, 0.8);
  background-color: $light-blue;
  border: 1px solid transparent;
  outline: none;

  &:focus {
    border-color: rgba($pink, 0.3);
  }
}
</style>

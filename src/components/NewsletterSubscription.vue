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
    margin-bottom: 3rem;
  }

  .btn {
    white-space: nowrap;
  }
}

.form-field {
  margin-right: 0.4rem;
}

.form-label {
  display: none;
}
.form-input {
  font-size: 1rem;
  font-family: inherit;
  font-weight: 300;
  padding: 0.4em 1em;
  border-radius: 100px;
  color: rgba($white, 0.8);
  background-color: $light-blue;
  border: 1px solid transparent;
  outline: none;
  width: 100%;

  &:focus {
    border-color: rgba($pink, 0.3);
  }
}

@media only screen and (min-width: "768px") {
  .newsletter {
    margin-left: auto;
    &-form {
      display: flex;
      margin-bottom: 5rem;
    }
  }
  .form-field {
    margin-right: 0.6rem;
    flex-basis: 80%;
  }

  .btn {
    font-size: 1rem;
  }
}

@media only screen and (min-width: "850px") {
  .newsletter {
    &-form {
      margin-bottom: 0;
    }
  }
}
</style>

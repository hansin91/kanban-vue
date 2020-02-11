<template>
  <form class="form-login">
    <h1 class="h3 mb-3 font-weight-normal">Please sign in</h1>
    <input
      type="email"
      id="inputEmail"
      class="form-control"
      :email="email"
      placeholder="Email address"
      required
      autofocus
    />
    <input type="password" id="inputPassword" class="form-control" placeholder="Password" required />
    <div class="checkbox mb-3">
      <label>
        <input type="checkbox" value="remember-me" /> Remember me
      </label>
    </div>
    <button class="btn btn-lg btn-primary btn-block" type="submit">Sign in</button>
    <p class="mt-5 mb-3 text-muted">© 2017-2019</p>
  </form>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      email: ""
    };
  }
};
</script>

<style lang="scss" scoped>
.form-login {
  width: 100%;
  max-width: 330px;
  padding: 15px;
  margin: auto;
}
</style>
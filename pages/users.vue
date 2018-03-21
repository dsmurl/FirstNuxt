<template>
  <section class="container">
    <div>

      <h1 class="title">
        Users
      </h1>

      <h2 class="subtitle">
        A simple list of users.
      </h2>

      <div class='user-form'>
        <input type="text" v-model="userId">
        <button @click="onLoadUser">Load User</button>
        <nuxt-child />
      </div>

      <div class="links">
        <nuxt-link to="/" class="button--green">Home</nuxt-link>
        <nuxt-link to="/users/123" class="button--green">User 123</nuxt-link>
      </div>

    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        userId: ''
      }
    },
    methods: {
      onLoadUser() {
        this.$router.push(`/users/${this.userId}`)
      }
    },
    layout: 'users',
  }
</script>


<style>
  .container
  {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
  .title
  {
    font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }
  .subtitle
  {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }
  .links a
  {
    margin: 5px;
  }
  .user-form {
    margin: 5px;
  }
</style>

<template>
  <section class="container">
    <div>
      <Header />
      <Logo/>
      <h1 class="title">
        first-nuxt
      </h1>
      <h2 class="subtitle">
        My premium Nuxt.js project
      </h2>
      <div class="links">
        <nuxt-link to="users" class="button--green">Users</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
  import Header from '~/components/Header.vue'
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo,
      Header
    }
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
</style>

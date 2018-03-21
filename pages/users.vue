<template>
  <div>
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
          <nuxt-link to="/users/123" class="button--green">User 123</nuxt-link>
        </div>

      </div>
    </section>
  </div>
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
  }
</script>


<template>
    <section class="container">
      <div>
        <Logo/>
        <h1 class="title">
          first-nuxt
        </h1>
        <h2 class="subtitle">
          My premium Nuxt.js project
        </h2>
      </div>
    </section>
</template>


<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo,
    }
  }
</script>


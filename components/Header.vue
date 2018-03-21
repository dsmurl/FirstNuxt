<template>
  <header class='header'>
    <ul class='nav-items'>
      <li class='nav-item'>
        <nuxt-link to='/' class="button--green">Home</nuxt-link>
      </li>
      <li class='nav-item'>
        <nuxt-link to='/users' class="button--green">Users</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<style scoped>
  .header {
    width: 100%;
    height: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #4870ff;
  }
  .nav-items {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 80%;
  }
</style>

<template>
    <div>
      <h2>
        User {{ $route.params.id }}<br />
        Name {{ $route.params.id }}<br />
        Age {{ $route.params.id }}<br />
        Color {{ $route.params.id }}<br />
      </h2>
    </div>
</template>


<script>
  export default {
    validate(data) {
      console.log('data: ', data);
      return /^\d+$/.test(data.params.id);
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

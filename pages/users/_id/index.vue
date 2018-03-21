<template>
    <div>
      <div class="user-box">
        User: {{ $route.params.id }}<br />
        Name: {{ $route.params.id }}<br />
        Age: {{ $route.params.id }}<br />
        Color: {{ $route.params.id }}<br />
      </div>
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
  .user-box {
    border: 1px solid black;
    border-radius: 4px;
    padding: 5px;
    margin: 10px;
    text-align: left;
  }
</style>

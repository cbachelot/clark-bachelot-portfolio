<!-- the router outlet, where all matched components would ber viewed -->
<template>
  <div id="nav">
  <router-link v-bind:to="'/'">Home</router-link>
  <router-link v-bind:to="'/about'">About</router-link>
  </div>
</template>

<script>
export default {
  name: 'Nav'
}
</script>
<!-- styling for the component -->
<style>
#nav {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

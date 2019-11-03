<!-- the router outlet, where all matched components would ber viewed -->
<template>
  <div id="nav">
  <router-link v-bind:to="'/'">Home</router-link>
  <router-link v-bind:to="'/about'">About</router-link>
  <transition
        name="fade"
        mode="out-in"
        @beforeLeave="beforeLeave"
        @enter="enter"
        @afterEnter="afterEnter"
      >
  <router-view></router-view>
  </transition>
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

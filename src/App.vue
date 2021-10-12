<script>
import { defineAsyncComponent } from 'vue'
export default {
  components: {
    Navbar: defineAsyncComponent(() =>
      import('./modules/dashboard/components/NavBar.vue')
    ),
  },
  setup() {},
}
</script>

<template>
  <h1>Weather App</h1>
  <Navbar />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

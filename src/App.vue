<template>
  <main>
    <HomePage/>
  </main>
</template>

<script>
import HomePage from './components/HomePage.vue'

export default {
  name: 'App',
  components: {
    HomePage
  }
}
</script>

<style>
  body{
    background-color:linen;
  }
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  }
</style>

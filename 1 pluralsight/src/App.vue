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
    background: linear-gradient(to bottom, rgb(218, 196, 174), linen);
  }
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  }
  main{
    margin: 0 auto;
    background-color: white;
    widows: 1024px;
    min-height: 300px;
  }
</style>

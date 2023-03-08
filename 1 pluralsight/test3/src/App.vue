<script>
import heroes from './components/heroesTT.vue'

export default {
  name: 'App',
  components: {
    heroes,
  }
}
</script>

<template>
  <heroes />
</template>

<style lang="scss">
@import "@/design/index.scss";
</style>

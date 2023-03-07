<script>
import counter from "./components/BaseCounter.vue";
import rondomNumbers from "./components/rondomNumbers.vue";
import characterList from "./components/characterList.vue";
import listCharacter from "./components/listCharacter.vue";
import barLinks from "./components/header-bar-links.vue";
import Heroes from "./components/heroesApp.vue";

export default {
  components: {
    Heroes,
    barLinks,
    counter,
    rondomNumbers,
    characterList,
    listCharacter,
  },
  data: () => ({
    newCharacter: {
      name: "",
      element: [],
    },
    favoriteList: [],
  }),
};
</script>

<template>
  <Heroes />
  <barLinks />
  <listCharacter />
  <characterList />
  <rondomNumbers />
  <counter />
</template>

<style lang="scss">
@import "@/design/index.scss";
@import "~bootstrap/dist/css/bootstrap.css";
</style>

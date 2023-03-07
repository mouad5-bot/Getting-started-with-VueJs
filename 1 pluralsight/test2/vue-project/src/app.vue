<script>
import HeaderBar from "@/components/header-bar";
import Heroes from "@/components/heroes";

export default {
  name: "App",
  components: { HeaderBar, Heroes },
};
</script>

<template>
  <div id="app">
    <HeaderBar />
    <div class="main-section columns">
      <main class="column">
        <h1>test</h1>
        <Heroes />
      </main>
    </div>
  </div>
</template>

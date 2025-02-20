<script setup lang="ts">
import { RouterView } from 'vue-router'
import TopBar from './components/TopBar.vue'
</script>

<template>
  <div id="app">
    <TopBar />
    <RouterView />
  </div>
</template>

<style scoped>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

#app {
  display: flex;
  flex-direction: column;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>

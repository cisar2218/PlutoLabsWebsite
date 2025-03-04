<script setup lang="ts">
import { RouterView } from 'vue-router'
import TopBar from './components/TopBar.vue'
import PageFooter from './components/PageFooter.vue'
</script>

<template>
  <div id="app-container">
    <TopBar />
    <RouterView />
    <PageFooter />
  </div>
</template>

<style scoped>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

#app-container {
  padding-top: 64px;
  display: flex;
  flex-direction: column;
  justify-content: center; /* Centers child horizontally */
  width: 100%;
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

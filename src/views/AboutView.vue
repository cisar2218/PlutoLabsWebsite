<script setup lang="ts">
import TeamSection from '../components/TeamSection.vue'
</script>

<template>
  <div class="about">
    <h1>Mission</h1>
    <p>
      something something something something something something something something something
      something something something something something something something something something
      something something something something something something something something something
      something something something something something something something something something
      something something something something something something something something something
      something something something something something something something
    </p>

    <h1>Team</h1>

    <TeamSection />
  </div>
</template>

<style>
h1 {
  margin-top: 20px;
  margin-bottom: 50px;
}

.about {
  display: flex;
  flex-direction: column;
  height: 100vh;
  padding: 100px 50px 0 50px;
  /* align-items: flex-start; */
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    /* align-items: center; */
  }
}
</style>

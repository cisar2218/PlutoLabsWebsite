<script setup lang="ts">
import CardRosta from '../components/team/CardRosta.vue'
import CardDusan from '../components/team/CardDusan.vue'
import CardDan from '../components/team/CardDan.vue'
</script>

<template>
  <div class="team-members">
    <CardRosta />
    <CardDan />
    <CardDusan />
  </div>
</template>

<style scoped>
.team-members {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  align-items: center;
}

@media (min-width: 1024px) {
  .team-members {
    display: flex;
    flex-direction: row;
    gap: 2rem;
  }
}
</style>

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
  flex-direction: row; /* Stack items vertically */
  gap: 20px; /* Space between each item */
}
</style>

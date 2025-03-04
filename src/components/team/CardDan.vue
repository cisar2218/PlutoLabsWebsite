<script setup lang="ts">
import CardTeamMember from '@/components/CardTeamMember.vue'
import danImage from '@/assets/photos/dan.jpg'
</script>

<template>
  <CardTeamMember
    name="Daniel Vaculík"
    :image="danImage"
    position="Marketing, sales, co-founder"
    link="https://www.linkedin.com/in/janesmith"
  />
</template>

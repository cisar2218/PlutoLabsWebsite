<script setup lang="ts">
import CardTeamMember from '@/components/CardTeamMember.vue'
import rostaImage from '@/assets/photos/rosta.jpg'
</script>

<template>
  <CardTeamMember
    name="Rostislav Litovkin"
    :image="rostaImage"
    position="CEO"
    link="https://www.linkedin.com/in/janesmith"
    linkdesc="Portfolio"
  />
</template>

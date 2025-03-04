<script setup lang="ts">
import CardTeamMember from '@/components/CardTeamMember.vue'
import dusanImage from '@/assets/photos/dusan.jpeg'
</script>

<template>
  <CardTeamMember
    name="Dušan Jánsky"
    :image="dusanImage"
    position="Developer, co-founder"
    link="https://www.github.com/cisar2218"
    linkdesc="GitHub"
  />
</template>

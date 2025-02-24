<script setup lang="ts">
import IconGithub from '@/components/icons/IconGithub.vue'
import IconDocumentation from '@/components/icons/IconDocumentation.vue'
import IconTooling from '@/components/icons/IconTooling.vue'
import CardResource from '@/components/CardResource.vue'
</script>

<template>
  <div class="about">
    <h1>PlutoFramework</h1>

    <div class="list">
      <CardResource
        title="Getting Started"
        text="get started by visiting the official documentation..."
      >
        <template #icon>
          <IconDocumentation class="icon" />
        </template>
      </CardResource>

      <div class="list-vertical">
        <IconGithub class="icon" />
      </div>

      <IconTooling class="icon" />
    </div>

    <h1>Team</h1>
    <p>something something</p>
  </div>
</template>

<style scoped>
.list {
  display: flex;
  flex-direction: row;
}

.icon {
  background-color: white;
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>

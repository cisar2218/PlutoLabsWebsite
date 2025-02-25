<script setup lang="ts">
import IconGithub from '@/components/icons/IconGithub.vue'
import IconDocumentation from '@/components/icons/IconDocumentation.vue'
import CardResource from '@/components/CardResource.vue'
</script>

<template>
  <div class="about">
    <h1>PlutoFramework</h1>

    <div class="list">
      <CardResource class="resource-card" title="Getting Started" link="https://plutolabs.gitbook.io/plutoframework"
        text="Get started by visiting the official documentation...">
        <template #icon>
          <IconDocumentation />
        </template>
      </CardResource>

      <CardResource class="resource-card" title="PlutoFramework Codebase"
        link="https://github.com/RostislavLitovkin/plutoframework"
        text="Are you ready? Use and Explore Pluto FrameWork. It's Open Source. ||| Are you ready? Use and Explore Pluto FrameWork. It's Open Source.">
        <template #icon>
          <IconGithub />
        </template>
      </CardResource>
    </div>
  </div>
</template>

<style>
.about {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  /* padding: 64px 50px 0 50px; */
  width: 100% !important;
  min-width: 100%;
  max-width: none;
  margin: 0;
  /* align-items: flex-start; */
}

html,
body,
#app {
  width: 100%;
  margin: 0;
  padding: 0;
}

.list {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 2rem;
  width: 100%;
  padding-left: 3rem;
  padding-right: 3rem;
}

.resource-card {
  flex: 1 1 100%;
  /* Each card takes full width on small screens */
  max-width: 600px;
}

.resource-card {
  flex: 1 1 90%;
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }

  .resource-card {
    flex: 1 1 30%;
    width: 30%;
  }
}
</style>

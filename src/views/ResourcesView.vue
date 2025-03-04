<script setup lang="ts">
import IconGithub from '@/components/icons/IconGithub.vue'
import IconDocumentation from '@/components/icons/IconDocumentation.vue'
import CardResource from '@/components/CardResource.vue'
</script>

<template>
  <div class="page">
    <h1>PlutoFramework</h1>

    <div class="list">
      <CardResource
        class="resource-card"
        title="Getting Started"
        link="https://plutolabs.gitbook.io/plutoframework"
        text="Get to know how to use PlutoFramework."
      >
        <template #icon>
          <IconDocumentation />
        </template>
      </CardResource>

      <CardResource
        class="resource-card"
        title="PlutoFramework Codebase"
        link="https://github.com/RostislavLitovkin/plutoframework"
        text="All in one framework for creating web3 mobile applications."
      >
        <template #icon>
          <IconGithub />
        </template>
      </CardResource>
    </div>

    <h1>Do you need a custom dApp?</h1>

    <p>
      We can build custom dApp for you as a service. See
      <RouterLink to="/" class="nav-item">solutions</RouterLink>.
    </p>
  </div>
</template>

<style>
html,
body,
#app {
  width: 100%;
  margin: 0;
  padding: 0;
}

.list {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
  width: 100%;
  padding-left: 3rem;
  padding-right: 3rem;
}

.resource-card {
  flex: 1 1 100%;
  max-width: 30rem;
  width: 30rem;
}

@media (min-width: 1024px) {
  .list {
    justify-content: center;
    flex-direction: row;
  }

  .resource-card {
    flex: 1 1 20%;
    width: 20%;
  }
}
</style>

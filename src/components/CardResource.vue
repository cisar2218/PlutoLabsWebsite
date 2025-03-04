<template>
  <a :href="link" target="_blank" rel="noopener noreferrer" class="card">
    <div class="card-header">
      <div class="card-icon">
        <slot name="icon"></slot>
        <!-- Slot for the icon -->
      </div>
    </div>

    <div class="card-botton">
      <h3 class="card-title">{{ title }}</h3>
      <p class="card-text">{{ text }}</p>
    </div>
  </a>
</template>

<script lang="ts">
export default {
  name: 'ResourceCard',
  props: {
    title: {
      type: String,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },
    link: {
      type: String,
      required: true,
    },
  },
}
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2rem;
  border: 1px solid #ddd;
  border-radius: 8px;
  height: 100%;
  width: 30rem;
}

.card:hover {
  background-color: var(--vt-c-indigo);
}

.card-header {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.card-icon {
  width: 3rem;
  height: 3rem;
}

.card-bottom {
  flex: 2;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.card-icon {
  width: 10rem;
  height: 10rem;
}

.card-title {
  display: flex;
  align-items: flex-start;
}

.card-text {
  min-height: 6rem;
  display: flex;
  align-items: flex-start;
}
</style>

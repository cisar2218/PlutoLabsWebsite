<template>
  <div class="card">
    <div class="card-icon">
      <slot name="icon"></slot>
      <!-- Slot for the icon -->
    </div>
    <h3 class="card-title">{{ title }}</h3>
    <p class="card-text">{{ text }}</p>
  </div>
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
  },
}
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 16px;
  border: 1px solid #ddd;
  border-radius: 8px;
  width: 200px;
}

.card-icon {
  font-size: 32px;
  margin-bottom: 8px;
}
</style>

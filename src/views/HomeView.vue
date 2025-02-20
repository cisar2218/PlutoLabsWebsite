<script setup lang="ts"></script>

<template>
  <div class="services">
    <h1>Services</h1>

    <div class="container">
      <div class="img-container">image</div>
      <div class="card-content">
        <div>name</div>
        <div>description</div>
      </div>
    </div>
    <div class="container"></div>
    <div class="container"></div>
  </div>
</template>

<style scoped>
.services {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}

.card-content {
  display: flex;
  flex-direction: column;
}

.img-container {
  position: relative;
  width: 50%;
  background-color: red;
}

.container {
  width: 50vw; /* Adjust width as needed */
  height: 300px;
  border: 1px solid #ccc;

  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  background-color: #ffffffa4;
  display: flex;
  flex-direction: row;
}
</style>

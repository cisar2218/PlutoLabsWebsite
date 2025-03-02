<template>
  <div class="card">
    <div class="img-container">
      <img src="@/assets/logo.svg" alt="Custom dApp Development" />
    </div>
    <div class="card-content">
      <h2>Custom dApp Development</h2>
      <h3>Why choose us?</h3>
      <p>
        Unlock the full potential of decentralized applications with our expert development
        services. Tailored to your unique needs, we ensure a seamless and efficient process from
        start to finish.
      </p>
      <h3>How it works:</h3>
      <ol>
        <li>Share your design and features with the Pluto Labs team.</li>
        <li>We'll propose a timetable and pricing.</li>
        <li>Development begins! We'll keep you updated throughout the process.</li>
        <li>Your custom dApp is ready for launch!</li>
      </ol>
    </div>
  </div>
</template>

<style scoped>
.card {
  display: flex;
  flex-direction: row;
  border: 1px solid #ccc;
  border-radius: 0; /* Sharp edges */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  margin-bottom: 2rem;
}

.img-container {
  flex: 1;
  background-color: #f0f0f0;
}

.img-container img {
  width: 100%;
  height: auto;
}

.card-content {
  flex: 2;
  padding: 1rem;
  display: flex;
  flex-direction: column;
}

@media (max-width: 768px) {
  .card {
    flex-direction: column;
  }

  .img-container {
    width: 100%;
  }
}
</style>

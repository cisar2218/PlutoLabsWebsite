<template>
  <div class="card">
    <div class="img-container">
      <img src="@/assets/logo.svg" alt="Custom dApp Development" />
    </div>
    <div class="card-content">
      <h2>Custom dApp Development</h2>
      <h3>Build the Future of Web3 with Pluto Labs</h3>
      <p>
        Unlock the full potential of decentralized applications with our expert-driven, tailor-made
        development services. Whether you're launching a new dApp or enhancing an existing one, we
        ensure a seamless, efficient, and secure development process from start to finish.
      </p>
      <h3>Why Choose Pluto Labs?</h3>
      <ul>
        <li>Custom Solutions: We adapt to your unique vision and technical needs.</li>
        <li>Expert Developers: Our team specializes in cutting-edge blockchain technologies.</li>
        <li>
          Transparent Process: Clear timelines, upfront pricing, and regular progress updates.
        </li>
        <li>Seamless Deployment: We ensure your dApp is optimized for a smooth launch.</li>
      </ul>

      <h3>How It Works</h3>
      <ol>
        <li>Share Your Vision: Tell us about your design, features, and goals.</li>
        <li>Receive a Plan: We provide a detailed roadmap, including timelines and pricing.</li>
        <li>Development in Action: Our team brings your dApp to life with regular updates.</li>
        <li>Launch & Scale: Your custom dApp is ready for deployment and future growth!</li>
      </ol>
    </div>
  </div>
</template>

<style scoped>
ul {
  position: relative;
  list-style: none;
  margin-left: 0;
  padding-left: 1.2em;
}

ul li::before {
  content: '🚀';
  position: absolute;
  left: 0;
}

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

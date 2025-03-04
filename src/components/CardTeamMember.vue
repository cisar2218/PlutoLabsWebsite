<template>
  <div class="team-card">
    <img :src="image" alt="Team Member" class="team-img" />
    <div class="team-info-overlay">
      <h2 class="team-name">{{ name }}</h2>
      <p class="team-position">{{ position }}</p>
      <a class="team-link" :href="link" target="_blank">{{ linkdesc }}</a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'TeamCard',
  props: {
    name: {
      type: String,
      required: true,
    },
    image: {
      type: String,
      required: true,
    },
    position: {
      type: String,
      required: true,
    },
    link: {
      type: String,
      required: true,
    },
    linkdesc: {
      default: 'LinkedIn',
      type: String,
      required: true,
    },
  },
}
</script>

<style scoped>
h1,
p {
  text-align: left;
}

.team-card {
  width: 26vh;
  border: 1px solid #ccc;
  height: 28rem;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  background-color: #ffffffa4;
  display: flex;
  flex-direction: column-reverse;
  position: relative;
}

.team-img {
  width: 100%;
  height: 100%;
  position: absolute;
  object-fit: cover;
}

.team-info-overlay {
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(255, 255, 255, 0.196);
  padding: 15px;
  height: 30%;
  backdrop-filter: blur(2px);
}

.team-info {
  display: flex;
  flex-direction: column;
  padding: 15px;
}

.team-name {
  color: var(--vt-c-text-dark-2);
  text-shadow: 1px 1px #000000;
  font-weight: bold;
  font-size: 1.2rem;
  margin: 0;
}

.team-position {
  font-style: italic;
  color: #777;
  margin: 5px 0;
}

.team-link {
  text-decoration: none;
  color: #007bff;
  font-weight: bold;
  padding-top: 1rem;
}

.team-link:hover {
  text-decoration: underline;
}

@media (min-width: 1024px) {
  .team-card {
    width: 26rem;
  }
}
</style>

<template>
  <div class="team-card">
    <img :src="image" alt="Team Member" class="team-img" />
    <div class="team-info">
      <h2 class="team-name">{{ name }}</h2>
      <p class="team-position">{{ position }}</p>
      <p class="team-description">{{ description }}</p>
      <a :href="link" target="_blank" class="team-link">{{ linkdesc }}</a>
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
    description: {
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
  width: 30%;
  /* Adjust width as needed */
  border: 1px solid #ccc;

  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  background-color: #ffffffa4;
  display: flex;
  flex-direction: column;
}

.team-img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  /* Ensures image is square and covers the area */
}

.team-info {
  padding: 15px;
}

.team-name {
  color: black;
  font-weight: bold;
  font-size: 1.2rem;
  margin: 0;
}

.team-position {
  font-style: italic;
  color: #777;
  margin: 5px 0;
}

.team-description {
  font-size: 0.95rem;
  color: #333;
  margin: 10px 0;
  height: 2rem;
}

.team-link {
  text-decoration: none;
  color: #007bff;
  font-weight: bold;
}

.team-link:hover {
  text-decoration: underline;
}
</style>

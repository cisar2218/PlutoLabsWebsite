<script lang="ts" setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
</script>


<template>
  <header class="topbar">
    <!-- Company Logo -->
    <div class="logo">
      <img src="@/assets/white_logo.svg" alt="Company Logo" />
      <span class="company-name">Pluto Labs</span>
    </div>

    <!-- Hamburger Icon for Mobile -->
    <div class="hamburger" @click="toggleMenu">
      <span></span>
      <span></span>
      <span></span>
    </div>

    <nav class="nav-links" :class="{ 'active': isMenuOpen }">
      <!-- Navigation Links -->
      <RouterLink to="/" class="nav-item">Solutions</RouterLink>
      <RouterLink to="/resources" class="nav-item">Resources</RouterLink>
      <RouterLink to="/about" class="nav-item">About Us</RouterLink>
    </nav>
  </header>
</template>

<style scoped>
/* Basic Styling for Top Bar */
.topbar {
  position: fixed;
  /* Fixes the navbar at the top of the page */
  top: 0;
  /* Aligns it to the top of the page */
  left: 0;
  /* Aligns it to the left of the page */
  width: 100%;
  /* Makes the navbar span the entire width */
  padding: 1rem 2rem;
  z-index: 1000;
  /* Ensures the navbar stays on top of other elements */
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #282c34;
  /* Dark background */
  color: white;
}


.logo {
  display: flex;
  align-items: center;
}

.logo img {
  width: 40px;
  /* Adjust the size of your logo */
  height: 40px;
  margin-right: 10px;
}

.company-name {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 20px;
}

.nav-item {
  color: white;
  text-decoration: none;
  font-size: 1rem;
}

/* Add to your existing <style> section */
.hamburger {
  display: none;
  /* Hidden by default on desktop */
  flex-direction: column;
  justify-content: space-between;
  width: 30px;
  height: 21px;
  cursor: pointer;
  z-index: 1001;
}

.hamburger span {
  display: block;
  height: 3px;
  width: 100%;
  background-color: white;
  border-radius: 3px;
}

/* Media query for mobile screens */
@media (max-width: 768px) {
  .hamburger {
    display: flex;
    /* Show on mobile */
  }

  .nav-links {
    position: absolute;
    top: 0;
    right: -100%;
    flex-direction: column;
    background-color: #282c34;
    width: 70%;
    height: 100vh;
    padding-top: 60px;
    transition: right 0.3s ease;
  }

  .nav-links.active {
    right: 0;
  }

  .nav-item {
    padding: 15px 25px;
    width: 100%;
  }
}
</style>

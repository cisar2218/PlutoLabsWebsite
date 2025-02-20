<template>
  <header class="topbar">
    <!-- Company Logo -->
    <div class="logo">
      <!-- replace with png -->
      <img src="@/assets/logo.svg" alt="Company Logo" />
      <span class="company-name">Pluto Labs</span>
    </div>

    <nav class="nav-links">
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
  position: fixed; /* Fixes the navbar at the top of the page */
  top: 0; /* Aligns it to the top of the page */
  left: 0; /* Aligns it to the left of the page */
  width: 100%; /* Makes the navbar span the entire width */
  z-index: 1000; /* Ensures the navbar stays on top of other elements */
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #282c34; /* Dark background */
  color: white;
}

.logo {
  display: flex;
  align-items: center;
}

.logo img {
  width: 40px; /* Adjust the size of your logo */
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
</style>

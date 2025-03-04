<script setup lang="ts">
const currentYear = new Date().getFullYear()
</script>

<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="social-links">
        <a
          href="https://t.me/+q3KX0kAPd8c0ZWU0"
          target="_blank"
          rel="noopener noreferrer"
          class="social-link"
        >
          <i class="fab fa-telegram"></i>
          <span>Telegram</span>
        </a>
        <a
          href="https://x.com/PlutoFramework"
          target="_blank"
          rel="noopener noreferrer"
          class="social-link"
        >
          <i class="fab fa-x-twitter"></i>
          <span>PlutoFramework</span>
        </a>
        <a
          href="https://www.youtube.com/@rostadeveloper/videos"
          target="_blank"
          rel="noopener noreferrer"
          class="social-link"
        >
          <i class="fab fa-youtube"></i>
          <span>YouTube</span>
        </a>
        <a
          href="https://github.com/RostislavLitovkin/plutoframework"
          target="_blank"
          rel="noopener noreferrer"
          class="social-link"
        >
          <i class="fab fa-github"></i>
          <span>GitHub</span>
        </a>
      </div>
      <div class="copyright">© {{ currentYear }} Pluto Labs. All rights reserved.</div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #282c34;
  color: white;
  padding: 2rem 0;
  margin-top: auto;
  width: 100%;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}

.social-links {
  display: flex;
  gap: 2rem;
  flex-wrap: wrap;
  justify-content: center;
}

.social-link {
  color: white;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  transition: color 0.3s ease;
}

.social-link:hover {
  color: #64b5f6;
}

.social-link i {
  font-size: 1.5rem;
}

.copyright {
  font-size: 0.9rem;
  opacity: 0.8;
}

span {
  width: 100%;
}

@media (max-width: 768px) {
  .social-links {
    gap: 1rem;
  }

  .social-link span {
    display: none;
  }

  .social-link i {
    font-size: 1.8rem;
  }
}
</style>

<template>
  <footer>
    <div class="social-links">
      <a href="https://github.com/sherifKhamis" target="_blank">GitHub</a>
      <a href="linkedin.com/in/sherifkhamis70327" target="_blank">LinkedIn</a>
    </div>
    <div class="credits">
      <a href="https://github.com/sherifKhamis/portfolioWebsite.git" target="_blank">
        Designed & Built by Sherif Khamis
      </a>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped>
footer {
  padding: 25px;
  text-align: center;
  font-family: 'Fira Code', monospace;
  font-size: 12px;
}

.social-links {
  margin-bottom: 15px;
}

.social-links a {
  margin: 0 10px;
  color: #8892b0;
  text-decoration: none;
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: #ffca28;
}

.credits a {
  color: #8892b0;
  text-decoration: none;
}

@media (max-width: 768px) {
  .social-links {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
}
</style>

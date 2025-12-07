<template>
  <header>
    <nav class="nav" aria-label="Hauptnavigation">
      <div class="nav-left">
        <ol>
          <li><a href="#about">Über mich</a></li>
          <li><a href="#experience">Erfahrung</a></li>
          <li><a href="#projects">Projekte</a></li>
          <li><a href="#contact">Kontakt</a></li>
        </ol>
      </div>
      <a :href="resumeHref" target="_blank" rel="noopener noreferrer" class="resume-button">Lebenslauf</a>
    </nav>
  </header>
</template>

<script setup>
// Robustes Lesen von BASE_URL (Vite) mit Fallback '/'
const base = (typeof import.meta !== 'undefined' && import.meta.env && import.meta.env.BASE_URL)
  ? import.meta.env.BASE_URL
  : '/'

const resumeHref = `${base}Sherif-Khamis-CV.pdf`
</script>

<style scoped>
header {
  background-color: #ffca28; /* Navbar-Farbe wie gewünscht */
  padding: 20px;
  position: relative;
  z-index: 10;
}

.nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
}

.nav-left ol {
  display: flex;
  gap: 20px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-left a {
  color: #0a192f;
  text-decoration: none;
  font-weight: 500;
}

.resume-button {
  border: 1px solid #0a192f;
  border-radius: 6px;
  padding: 10px 16px;
  color: #0a192f;
  text-decoration: none;
  background: transparent;
  margin-left: 24px; /* zusätzlicher Abstand zur Navigation */
  white-space: nowrap;
}

@media (max-width: 640px) {
  .nav {
    flex-direction: column;
    align-items: stretch;
  }
  .nav-left ol {
    justify-content: center;
    flex-wrap: wrap;
    gap: 12px;
  }
  .resume-button {
    align-self: center;
    margin-top: 12px;
  }
}
</style>

<template>
  <header>
    <nav>
      <ol>
        <li><a href="#about">Über mich</a></li>
        <li><a href="#experience">Erfahrung</a></li>
        <li><a href="#projects">Projekte</a></li>
        <li><a href="#contact">Kontakt</a></li>
      </ol>
      <a href="../../public/Sherif%20Khamis%20-%20CV.pdf" target="_blank" class="resume-button">Resume</a>
    </nav>
  </header>
</template>

<script setup>
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background-color: #ffca28;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

nav ol {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

nav li {
  margin-left: 20px;
}

nav a {
  color: #0a192f;
  text-decoration: none;
}

.resume-button {
  border: 1px solid #0a192f;
  border-radius: 4px;
  padding: 10px 15px;
  color: #0a192f;
  text-decoration: none;
  margin-left: 20px; /* Fügt Abstand hinzu */
}
</style>

<template>
  <section id="intro">
    <p class="hi">Hallo, mein Name ist</p>
    <h1 class="name">Sherif Khamis.</h1>
    <h2 class="subtitle">Ich brenne für Software Engineering & Data Science</h2>
    <p class="description">
      Meine Leidenschaft für die Schnittstelle von Software Engineering und Data Science hat mein gesamtes Informatikstudium geprägt.
      Jetzt, als Absolvent, möchte ich diese Begeisterung nutzen, um aus komplexen Datensätzen intelligente und performante Anwendungen zu entwickeln.
    </p>
    <a href="#projects" class="cta-button">Zu meinen Projekten</a>
  </section>
</template>

<script setup>
</script>

<style scoped>
#intro {
  padding: 100px 0;
}

.hi {
  color: #ffca28;
  font-family: 'Fira Code', monospace;
}

.name {
  color: #ccd6f6;
  font-size: 80px;
  font-weight: 600;
  margin: 0;
}

.subtitle {
  color: #8892b0;
  font-size: 70px;
  font-weight: 600;
  margin-top: 10px;
}

.description {
  margin-top: 25px;
  max-width: 540px;
}

.cta-button {
  display: inline-block;
  margin-top: 50px;
  padding: 20px 30px;
  border: 1px solid #ffca28;
  border-radius: 4px;
  color: #ffca28;
  text-decoration: none;
}

@media (max-width: 1024px) {
  .name {
    font-size: 70px;
  }
  .subtitle {
    font-size: 60px;
  }
}

@media (max-width: 768px) {
  #intro {
    padding: 80px 0;
  }
  .name {
    font-size: 50px;
  }
  .subtitle {
    font-size: 40px;
  }
}

@media (max-width: 480px) {
  #intro {
    padding: 60px 0;
  }
  .name {
    font-size: 40px;
  }
  .subtitle {
    font-size: 30px;
  }
  .description {
    max-width: 100%;
  }
}
</style>

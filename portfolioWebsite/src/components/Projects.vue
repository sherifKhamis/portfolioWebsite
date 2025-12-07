<template>
  <section id="projects">
    <h2 class="section-heading">Meine Projekte</h2>
    <div class="in-progress-container">
      <p>Derzeit in Entwicklung... Schaue bald wieder vorbei!</p>
      <div class="loader"></div>
    </div>
  </section>
</template>

<script setup>
// Für diese Ansicht ist keine Skriptlogik erforderlich.
</script>

<style scoped>
#projects {
  padding: 100px 0;
  text-align: center;
}

.section-heading {
  color: #ccd6f6;
  font-size: 32px;
  font-weight: 600;
  margin-bottom: 40px;
}

.in-progress-container {
  background-color: #112240;
  padding: 50px;
  border-radius: 4px;
  color: #a8b2d1;
  max-width: 700px;
  margin: 0 auto;
}

.in-progress-container p {
  font-size: 18px;
  margin-bottom: 30px;
}

.loader {
  border: 4px solid #233554;
  border-left-color: #ffca28;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  animation: spin 1s linear infinite;
  margin: 0 auto;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
</style>


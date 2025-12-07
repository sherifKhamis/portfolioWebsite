<template>
  <section id="about">
    <h2 class="section-heading">Über mich</h2>
    <div class="content">
      <div class="text">
        <p>
          Hallo, ich bin Sherif, Informatik Absolvent, wohnhaft in nähe Stuttgart.
          Mir macht es Spaß, Software zu entwickeln und große Datenmengen zu analysieren. Ebenso baue
          ich gerne ETL-Pipelines welche diese Datenanalye erst ermöglichen.
        </p>
        <p>
          Ich habe sowohl eine Ausbildung als auch ein Bachelorstudium im Bereich Informatik abgeschlossen. Und suche
          nach einer Festanstellung im Bereich Software Engineering oder Data Science.
        </p>

        <p>
          Meine Ausbildung habe ich in Kooperation mit der Mercedes-Benz AG abgeschlossen. Und das Studium größtenteils
          parallel an der IU Internationalen Hochschule.
        </p>

        <p>Hier sind ein paar Technologien, mit denen ich kürzlich gearbeit habe:</p>
        <ul>
          <li>JavaScript</li>
          <li>Vue.js</li>
          <li>Python</li>
          <li>HTML & CSS</li>
          <li>Java</li>
          <li>SQL</li>
        </ul>
      </div>
      <div class="image-wrapper">
        <img src="../../public/Sherif_Khamis.jpeg" alt="Sherif Khamis" />
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
#about {
  padding: 100px 0;
}

.section-heading {
  color: #ccd6f6;
  font-size: 32px;
  font-weight: 600;
  margin-bottom: 40px;
}

.content {
  display: grid;
  grid-template-columns: 3fr 2fr;
  gap: 50px;
}

ul {
  display: grid;
  grid-template-columns: repeat(2, minmax(140px, 200px));
  gap: 0px 10px;
  padding: 0px;
  margin: 20px 0px 0px;
  overflow: hidden;
  list-style: none;
}

li {
  position: relative;
  margin-bottom: 10px;
  padding-left: 20px;
  font-family: 'Fira Code', monospace;
}

li::before {
  content: "▹";
  position: absolute;
  left: 0px;
  color: #ffca28;
}

.image-wrapper {
  position: relative;
  max-width: 300px;
}

img {
  width: 100%;
  border-radius: 4px;
}

@media (max-width: 768px) {
  .content {
    grid-template-columns: 1fr;
    gap: 30px;
  }
  .image-wrapper {
    max-width: 250px;
    margin: 0 auto;
  }
  #about {
    padding: 80px 0;
  }
}

@media (max-width: 480px) {
  ul {
    grid-template-columns: 1fr;
  }
  #about {
    padding: 60px 0;
  }
}
</style>

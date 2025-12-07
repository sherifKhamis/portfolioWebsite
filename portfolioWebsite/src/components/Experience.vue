<template>
  <section id="experience">
    <h2 class="section-heading">Meine bisherigen Positionen</h2>
    <div class="tabs">
      <div class="tab-list" role="tablist">
        <button
          v-for="(job, index) in jobs"
          :key="index"
          class="tab"
          :class="{ active: activeTab === index }"
          @click="activeTab = index"
        >
          {{ job.company }}
        </button>
      </div>
      <div class="tab-panel">
        <div v-if="activeJob">
          <h3>
            <span>{{ activeJob.title }}</span>
            <span class="company">
              &nbsp;@&nbsp;
              <a :href="activeJob.url" target="_blank">{{ activeJob.company }}</a>
            </span>
          </h3>
          <p class="range">{{ activeJob.range }}</p>
          <ul>
            <li v-for="(item, i) in activeJob.duties" :key="i">{{ item }}</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, computed } from 'vue';

const activeTab = ref(0);

const jobs = ref([
  {
    company: 'Mercedes-Benz AG',
    title: 'Bachelorand',
    url: 'https://group.mercedes-benz.com/de/',
    range: 'März 2026 - August 2026',
    duties: [
      'Analyse besteheder Datenquellen und -stukturen',
      'Entwicklung und Dokumentation eines semantischen Datenmodells für einen ausgewählten Anwendungsfall',
      'Identifikation und Modellierung von Entitäten, Relationen und Attributen',
      'Anwendung von Standards und Methoden der semantischen Datenmodellierung',
      'Zusammenarbeit mit Fachbereichen zur Erhebung und Abstimmung von Anforderungen',
      'Präsentation und Visualiserung des Modells für verschiedene Zielgruppen'
    ],
  },
  {
    company: 'Mercedes-Benz AG',
    title: 'Auszubildender Fachinformatiker für Daten- und Prozessanalyse',
    url: 'https://group.mercedes-benz.com/de/',
    range: 'September 2023 - Januar 2026',
    duties: [
      'Entwicklung einer End-to-End Datenpipeline zur Analyse von Fahrzeugsteuergerätedaten mittels MB.OS Data Collection Infrastruktur zur Identifikation von Buswachhaltern ',
      'Entwicklung und Wartung einer zentralen Webanwendungsplattform zur Verwaltung und Bereitstellung von Daten für Systeme des autonomen Fahrens ',
      'Entwicklung von Power-BI Dashboards, basierend auf Logistiklieferantendaten ',
      'Erstellung, Optimierung und Automatisierung von Skripten',
    ],
  },
]);

const activeJob = computed(() => jobs.value[activeTab.value]);
</script>

<style scoped>
#experience {
  padding: 100px 0;
  max-width: 700px;
  margin: 0 auto;
}

.section-heading {
  color: #ccd6f6;
  font-size: 32px;
  font-weight: 600;
  margin-bottom: 40px;
}

.tabs {
  display: flex;
  min-height: 340px;
}

.tab-list {
  display: flex;
  flex-direction: column;
}

.tab {
  background: none;
  border: none;
  border-left: 2px solid #233554;
  padding: 15px;
  color: #8892b0;
  cursor: pointer;
  text-align: left;
  font-family: 'Fira Code', monospace;
}

.tab.active {
  color: #ffca28;
  border-left-color: #ffca28;
  background-color: #112240;
}

.tab-panel {
  padding-left: 20px;
}

h3 {
  color: #ccd6f6;
  font-size: 22px;
}

.company {
  color: #ffca28;
}

.range {
  font-family: 'Fira Code', monospace;
  font-size: 13px;
  margin-bottom: 25px;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  position: relative;
  padding-left: 30px;
  margin-bottom: 10px;
}

li::before {
  content: "▹";
  position: absolute;
  left: 0px;
  color: #ffca28;
}
</style>


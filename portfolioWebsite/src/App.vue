<script setup>
import Header from './components/Header.vue';
import Intro from './components/Intro.vue';
import About from './components/About.vue';
import Experience from './components/Experience.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';
import './assets/main.css';
</script>

<template>
  <Header />
  <main>
    <Intro />
    <About />
    <Experience />
    <Projects />
    <Contact />
  </main>
  <Footer />
</template>

<style scoped>
main {
  padding: 0px 150px;
}
</style>

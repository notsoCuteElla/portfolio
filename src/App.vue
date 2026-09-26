<script setup lang="ts">
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="min-h-screen bg-cream text-dark-green">
    <Navbar />

    <main>
      <Hero />
      <About />
      <Skills />
      <Projects />
      <Contact />
    </main>

    <Footer />
  </div>
</template>

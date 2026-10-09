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
  <div class="relative min-h-screen text-white overflow-x-hidden">
    <!-- Global Background Video Loop for the Whole Website -->
    <div class="fixed inset-0 z-[-1] overflow-hidden">
      <video
        autoplay
        muted
        loop
        playsinline
        class="absolute inset-0 h-full w-full object-cover object-center"
      >
        <source src="/videos/background.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
      <!-- Balanced opacity overlay set to 65 -->
      <div class="absolute inset-0 bg-forest-950/65 backdrop-blur-[1px]"></div>
    </div>

    <!-- Main Application Flow -->
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

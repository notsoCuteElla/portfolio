<script setup lang="ts">
import ProjectCard from './ProjectCard.vue'

const projects = [
  {
    title: 'EcoFloat',
    description:
      'A smart floating waste collector designed to help collect floating solid waste from inland waterways.',
    technologies: ['ESP32', 'IoT', 'Computer Vision', 'Solar Power'],
    github: 'https://github.com/',
  },
  {
    title: 'WHEELGO',
    description:
      'A voice-controlled smart wheelchair concept with patient assistance, location monitoring, and emergency caregiver alerts.',
    technologies: ['ESP32', 'Voice Control', 'GPS', 'IoT'],
    github: 'https://github.com/',
  },
  {
    title: 'Smart Drainage Monitoring',
    description:
      'A multi-sensor monitoring concept designed to distinguish possible drainage clogging from high-water conditions.',
    technologies: ['ESP32', 'Sensors', 'Web Dashboard', 'Solar Power'],
    github: 'https://github.com/',
  },
]
</script>

<template>
  <section id="projects" class="px-6 py-24">
    <div class="mx-auto max-w-6xl">
      <p class="font-medium text-matcha-600">Projects</p>

      <h2 class="mt-2 text-3xl font-bold md:text-4xl">Selected Work</h2>

      <p class="mt-4 max-w-2xl text-dark-green/70">
        A selection of projects demonstrating my experience with software, web development, IoT, and
        emerging technologies.
      </p>

      <div class="mt-10 grid gap-6 md:grid-cols-2 lg:grid-cols-3">
        <ProjectCard v-for="project in projects" :key="project.title" v-bind="project" />
      </div>
    </div>
  </section>
</template>

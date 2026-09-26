<script setup lang="ts">
import ProjectCard from './ProjectCard.vue'

const projects = [
  {
    title: 'DiLiGaN',
    problem:
      'Urban areas lack real-time localized tracking of environmental conditions, soil moisture, and rainfall risks.',
    solution:
      'Built an urban monitoring system using multiple sensors to track soil status, water levels, and rain activity.',
    technologies: ['ESP32', 'IoT', 'Soil Sensor', 'Ultrasonic Sensor', 'Rain Sensor'],
    github: 'https://github.com/notsoCuteElla',
  },
  {
    title: 'Durian-Quiamco Dental Clinic',
    problem:
      'Dental clinics struggle with manual appointment scheduling, disorganized patient records, and tracking dental histories.',
    solution:
      'Developed a comprehensive web-based clinic management system to streamline appointment scheduling, patient records, and monitoring.',
    technologies: ['HTML', 'CSS', 'Node.js', 'JavaScript'],
    github: 'https://github.com/notsoCuteElla',
  },
  {
    title: 'RDCHelp_Desk',
    problem:
      'Technical support teams face delays and disorganization when tracking, prioritizing, and resolving user inquiries.',
    solution:
      'Built a centralized helpdesk ticketing system designed to log, track, and manage user support requests efficiently.',
    technologies: ['HTML', 'CSS', 'Node.js', 'JavaScript'],
    github: 'https://github.com/notsoCuteElla/rdchelp-desk',
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

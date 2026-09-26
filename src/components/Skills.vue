<script setup lang="ts">
const skills = [
  'HTML',
  'CSS',
  'JavaScript',
  'TypeScript',
  'Vue.js',
  'Tailwind CSS',
  'Git',
  'GitHub',
  'Python',
  'Django',
  'REST API',
]
</script>

<template>
  <section id="skills" class="bg-matcha-100 px-6 py-24">
    <div class="mx-auto max-w-6xl">
      <p class="font-medium text-matcha-700">Skills</p>

      <h2 class="mt-2 text-3xl font-bold md:text-4xl">Technologies I work with</h2>

      <div class="mt-8 flex flex-wrap gap-3">
        <span
          v-for="skill in skills"
          :key="skill"
          class="rounded-full border border-matcha-300 bg-cream px-4 py-2 text-sm font-medium"
        >
          {{ skill }}
        </span>
      </div>
    </div>
  </section>
</template>

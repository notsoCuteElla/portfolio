<script setup lang="ts">
defineProps<{
  title: string
  problem: string
  solution: string
  technologies: string[]
  github?: string
  demo?: string
  image?: string
}>()
</script>

<template>
  <article
    class="flex flex-col rounded-2xl border border-forest-100 bg-white overflow-hidden shadow-sm transition-all duration-300 hover:-translate-y-1 hover:shadow-xl hover:border-forest-300"
  >
    <!-- Project Preview Image (Optional) -->
    <div v-if="image" class="h-48 w-full bg-forest-100 overflow-hidden">
      <img
        :src="image"
        :alt="title"
        class="h-full w-full object-cover transition-transform duration-500 hover:scale-105"
      />
    </div>

    <div class="flex flex-1 flex-col p-6">
      <h3 class="text-xl font-bold text-forest-950">{{ title }}</h3>

      <div class="mt-4 space-y-2 text-sm text-forest-900/80 flex-1">
        <p><strong class="font-semibold text-forest-950">Problem:</strong> {{ problem }}</p>
        <p><strong class="font-semibold text-forest-950">Solution:</strong> {{ solution }}</p>
      </div>

      <!-- Tech Badges -->
      <div class="mt-6 flex flex-wrap gap-1.5">
        <span
          v-for="tech in technologies"
          :key="tech"
          class="rounded-md bg-forest-50 px-2.5 py-1 text-xs font-semibold text-forest-800 border border-forest-200/50"
        >
          {{ tech }}
        </span>
      </div>

      <!-- Action Links -->
      <div class="mt-6 flex items-center justify-between border-t border-forest-100 pt-4">
        <a
          v-if="github"
          :href="github"
          target="_blank"
          rel="noopener noreferrer"
          class="text-xs font-bold uppercase tracking-wider text-forest-700 hover:text-gold-accent transition"
        >
          View Source Code →
        </a>
        <a
          v-if="demo"
          :href="demo"
          target="_blank"
          rel="noopener noreferrer"
          class="text-xs font-bold uppercase tracking-wider text-forest-700 hover:text-gold-accent transition"
        >
          Live Preview ↗
        </a>
      </div>
    </div>
  </article>
</template>

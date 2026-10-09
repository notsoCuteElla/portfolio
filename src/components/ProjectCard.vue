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
    class="flex flex-col rounded-2xl border border-forest-700/50 bg-forest-900/80 backdrop-blur-md overflow-hidden shadow-xl transition-all duration-300 hover:-translate-y-1 hover:border-forest-500/70"
  >
    <!-- Project Preview Image (Optional) -->
    <div v-if="image" class="h-48 w-full bg-forest-950 overflow-hidden">
      <img
        :src="image"
        :alt="title"
        class="h-full w-full object-cover transition-transform duration-500 hover:scale-105 opacity-90"
      />
    </div>

    <div class="flex flex-1 flex-col p-6 text-white">
      <h3 class="text-xl font-bold text-cream-bg tracking-wide">{{ title }}</h3>

      <div class="mt-4 space-y-2 text-sm text-forest-200/90 flex-1 font-light">
        <p><strong class="font-semibold text-gold-accent">Problem:</strong> {{ problem }}</p>
        <p><strong class="font-semibold text-gold-accent">Solution:</strong> {{ solution }}</p>
      </div>

      <!-- Tech Badges -->
      <div class="mt-6 flex flex-wrap gap-1.5">
        <span
          v-for="tech in technologies"
          :key="tech"
          class="rounded-md bg-forest-950/60 px-2.5 py-1 text-xs font-semibold text-forest-200 border border-forest-700/60"
        >
          {{ tech }}
        </span>
      </div>

      <!-- Action Links -->
      <div class="mt-6 flex items-center justify-between border-t border-forest-800/80 pt-4">
        <a
          v-if="github"
          :href="github"
          target="_blank"
          rel="noopener noreferrer"
          class="text-xs font-bold uppercase tracking-wider text-gold-accent hover:underline transition"
        >
          View Source Code →
        </a>
        <a
          v-if="demo"
          :href="demo"
          target="_blank"
          rel="noopener noreferrer"
          class="text-xs font-bold uppercase tracking-wider text-gold-accent hover:underline transition"
        >
          Live Preview ↗
        </a>
      </div>
    </div>
  </article>
</template>

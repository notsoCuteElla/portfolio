<script setup lang="ts">
import profileImage from '../assets/profile.jpg'
</script>

<template>
  <section class="relative flex min-h-screen items-center px-6 pt-28 pb-16 overflow-hidden">
    <!-- Content Container -->
    <div class="relative z-10 mx-auto grid max-w-6xl items-center gap-12 lg:grid-cols-12 w-full">
      <!-- Text & Value Proposition -->
      <div class="lg:col-span-7 text-white">
        <div
          class="inline-flex items-center gap-2 rounded-full bg-forest-900/80 px-3.5 py-1 text-xs font-semibold uppercase tracking-wider text-forest-200 mb-6 border border-forest-700/60 shadow-md backdrop-blur-md"
        >
          <span class="h-2 w-2 rounded-full bg-gold-accent animate-pulse"></span>
          Available for Opportunities
        </div>

        <h1 class="text-4xl font-extrabold tracking-tight sm:text-6xl lg:text-7xl drop-shadow-md">
          Meca Ella <br />
          <span class="italic font-serif font-normal text-gold-accent">Paddanan</span>
        </h1>

        <p class="mt-4 text-xl font-medium text-forest-100 drop-shadow">
          Frontend Developer & IoT Solutions Specialist
        </p>

        <p class="mt-4 max-w-xl text-base leading-relaxed text-forest-200/90 drop-shadow">
          Crafting responsive, high-performance web applications and hardware-integrated software
          solutions. Focused on clean architecture, intuitive UX, and purposeful digital
          experiences.
        </p>

        <div class="mt-8 flex flex-wrap gap-4">
          <a
            href="#projects"
            class="rounded-xl bg-gold-accent px-7 py-3.5 text-sm font-semibold text-forest-950 shadow-lg transition hover:bg-yellow-400 hover:-translate-y-0.5"
          >
            Explore Projects →
          </a>

          <a
            href="#contact"
            class="rounded-xl border border-forest-400/30 bg-forest-900/40 px-7 py-3.5 text-sm font-semibold text-white backdrop-blur-md transition hover:bg-forest-800"
          >
            Get In Touch
          </a>
        </div>
      </div>

      <!-- Hero Visual Profile -->
      <div class="relative lg:col-span-5 flex justify-center">
        <div
          class="relative w-72 h-80 sm:w-80 sm:h-96 rounded-2xl overflow-hidden border-2 border-forest-300/40 shadow-2xl shadow-forest-950/60 bg-forest-900/40 backdrop-blur-md"
        >
          <img
            :src="profileImage"
            alt="Meca Ella Paddanan"
            class="w-full h-full object-cover object-center"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import logoImg from '../assets/logo.jpg'
</script>

<template>
  <nav
    class="fixed top-0 left-0 right-0 z-50 w-full border-b border-forest-700/50 bg-forest-900/90 backdrop-blur-md transition-all shadow-md"
  >
    <div class="mx-auto flex max-w-6xl items-center justify-between px-6 py-4">
      <!-- Logo Avatar + Name -->
      <a
        href="#"
        class="flex items-center gap-3 text-lg md:text-xl font-black tracking-tight text-white hover:opacity-90 transition"
      >
        <img
          :src="logoImg"
          alt="Logo"
          class="h-10 w-10 rounded-full object-cover border-2 border-gold-accent shadow-md"
        />
        <span>MECA ELLA PADDANAN<span class="text-gold-accent">.</span></span>
      </a>

      <!-- Navigation Links -->
      <div class="hidden gap-8 text-sm font-semibold tracking-wide text-forest-200 md:flex">
        <a href="#about" class="transition hover:text-gold-accent">ABOUT</a>
        <a href="#skills" class="transition hover:text-gold-accent">SKILLS</a>
        <a href="#projects" class="transition hover:text-gold-accent">PROJECTS</a>
        <a href="#contact" class="transition hover:text-gold-accent">CONTACT</a>
      </div>
    </div>
  </nav>
</template>

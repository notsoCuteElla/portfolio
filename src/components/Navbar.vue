<script setup>
import { ref } from 'vue'
import logoImg from '../assets/logo.jpg'

const isOpen = ref(false)

const navLinks = [
  { name: 'About', href: '#about' },
  { name: 'Projects', href: '#projects' },
  { name: 'Skills', href: '#skills' },
  { name: 'Contact', href: '#contact' },
]
</script>

<template>
  <header class="w-full bg-[#11221c] text-white fixed top-0 left-0 z-50 shadow-md">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
      <!-- Logo & Brand -->
      <div class="flex items-center space-x-3 min-w-0 pr-2">
        <img
          :src="logoImg"
          alt="Meca Ella Avatar"
          class="w-9 h-9 rounded-full object-cover shrink-0 border border-emerald-700/50 shadow-sm"
        />
        <span class="font-bold tracking-wider text-xs sm:text-sm md:text-base truncate">
          MECA ELLA PADDANAN
        </span>
      </div>

      <!-- Desktop Nav Links -->
      <nav class="hidden md:flex items-center space-x-6">
        <a
          v-for="link in navLinks"
          :key="link.name"
          :href="link.href"
          class="hover:text-amber-500 transition-colors"
        >
          {{ link.name }}
        </a>
      </nav>

      <!-- Hamburger Button (Mobile Only) -->
      <button
        @click="isOpen = !isOpen"
        class="md:hidden text-white focus:outline-none p-2 rounded-lg hover:bg-emerald-900/40 transition-colors shrink-0"
        aria-label="Toggle Menu"
      >
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path
            v-if="!isOpen"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          />
          <path
            v-else
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          />
        </svg>
      </button>
    </div>

    <!-- Mobile Dropdown Menu -->
    <div
      v-show="isOpen"
      class="md:hidden bg-[#11221c] border-t border-emerald-900/50 px-4 pt-2 pb-4 space-y-2 shadow-xl"
    >
      <a
        v-for="link in navLinks"
        :key="link.name"
        :href="link.href"
        @click="isOpen = false"
        class="block px-3 py-2.5 rounded-md text-base font-medium hover:bg-emerald-900/40 transition-colors"
      >
        {{ link.name }}
      </a>
    </div>
  </header>
</template>

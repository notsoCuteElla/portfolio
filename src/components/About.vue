<template>
  <section id="about" class="px-6 py-24 bg-white/60">
    <div class="mx-auto max-w-6xl">
      <div class="flex items-center gap-3">
        <div class="h-0.5 w-8 bg-gold-accent"></div>
        <span class="text-xs font-bold uppercase tracking-widest text-forest-700">About Me</span>
      </div>

      <h2 class="mt-3 text-3xl font-extrabold text-forest-950 md:text-4xl">
        Bridging Software Engineering & Practical Innovation
      </h2>

      <div class="mt-8 grid gap-10 md:grid-cols-12">
        <div class="md:col-span-7 space-y-4 text-base leading-relaxed text-forest-900/80">
          <p>
            I am a developer dedicated to engineering modern web interfaces and functional embedded
            systems. My background spans building clean, maintainable user interfaces with Vue 3 and
            TypeScript, alongside hardware-software integration using microcontrollers like ESP32.
          </p>
          <p>
            Whether designing responsive client dashboards or programming real-time sensor networks
            for environmental monitoring, my approach prioritizes reliability, usability, and
            sustainable system design.
          </p>
        </div>

        <!-- Key Pillars Grid -->
        <div class="md:col-span-5 grid gap-4 sm:grid-cols-2">
          <div class="rounded-xl border border-forest-100 bg-cream-bg p-5 shadow-sm">
            <div class="text-2xl mb-2">💻</div>
            <h3 class="font-bold text-forest-950">Frontend Dev</h3>
            <p class="mt-1 text-xs text-forest-800/70">
              Modern Vue 3 ecosystems, reactive state, and utility-first styling.
            </p>
          </div>

          <div class="rounded-xl border border-forest-100 bg-cream-bg p-5 shadow-sm">
            <div class="text-2xl mb-2">⚡</div>
            <h3 class="font-bold text-forest-950">IoT Integration</h3>
            <p class="mt-1 text-xs text-forest-800/70">
              Connecting hardware sensors, voice control, and web telemetry.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

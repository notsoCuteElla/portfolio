<template>
  <section id="contact" class="relative bg-forest-950 px-6 py-24 text-white overflow-hidden">
    <!-- Subtle Background Accent -->
    <div
      class="absolute -right-20 -bottom-20 h-96 w-96 rounded-full bg-forest-800/30 blur-3xl"
    ></div>

    <div class="relative mx-auto max-w-6xl">
      <div class="flex items-center gap-3">
        <div class="h-0.5 w-8 bg-gold-accent"></div>
        <span class="text-xs font-bold uppercase tracking-widest text-forest-300"
          >Get In Touch</span
        >
      </div>

      <h2 class="mt-3 text-3xl font-extrabold text-white md:text-5xl">
        Let’s Build Something Together
      </h2>

      <p class="mt-4 max-w-xl text-base text-forest-200/80">
        I am currently open to web development roles, IoT collaborations, and software engineering
        opportunities. Feel free to reach out via email or connect on GitHub.
      </p>

      <div class="mt-8 flex flex-wrap items-center gap-4">
        <a
          href="mailto:your-email@example.com"
          class="rounded-xl bg-gold-accent px-8 py-4 font-bold text-forest-950 transition hover:bg-yellow-400 hover:shadow-lg"
        >
          Send an Email
        </a>

        <a
          href="https://github.com/YOUR_USERNAME"
          target="_blank"
          rel="noopener noreferrer"
          class="rounded-xl border border-forest-700 px-8 py-4 font-bold text-white transition hover:bg-forest-900"
        >
          GitHub Profile
        </a>
      </div>
    </div>
  </section>
</template>

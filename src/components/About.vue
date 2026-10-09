<template>
  <section id="about" class="py-28 px-6 max-w-5xl mx-auto">
    <div class="relative">
      <!-- Natural Glow Backdrop -->
      <div
        class="absolute -inset-1 bg-gradient-to-r from-forest-600/20 to-gold-accent/10 rounded-3xl blur-2xl opacity-70"
      ></div>

      <div
        class="relative bg-forest-950/60 border border-forest-700/40 rounded-2xl p-8 md:p-12 backdrop-blur-xl shadow-2xl space-y-10 text-white"
      >
        <!-- Top Credential Badge -->
        <div
          class="flex flex-wrap items-center justify-between border-b border-forest-800/80 pb-6 gap-4"
        >
          <div>
            <p class="text-xs uppercase tracking-widest text-gold-accent font-semibold">
              Professional Credential
            </p>
            <p class="text-lg font-bold text-cream-bg mt-1">
              Civil Service Eligible - Professional Level
            </p>
          </div>
          <div
            class="rounded-xl bg-forest-900/80 px-4 py-2 border border-forest-700/60 text-xs font-medium text-forest-200"
          >
            Cagayan State University - Carig Campus
          </div>
        </div>

        <!-- Professional Summary -->
        <div>
          <h2
            class="text-xs uppercase tracking-widest font-semibold text-gold-accent mb-3 flex items-center gap-2"
          >
            <span>🌿</span> Professional Summary
          </h2>
          <p class="text-forest-200 leading-relaxed text-base md:text-lg font-light">
            An undergraduate Computer Engineering professional specializing in full-stack web
            development, embedded IoT hardware systems, and computer vision integration. Dedicated
            to engineering clean, sustainable, and high-performance technological solutions.
          </p>
        </div>

        <!-- Education & Background -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div class="bg-forest-900/40 p-6 rounded-xl border border-forest-800/60 space-y-2">
            <h2 class="text-xs uppercase tracking-widest font-semibold text-gold-accent">
              Education
            </h2>
            <p class="font-bold text-cream-bg">B.S. in Computer Engineering</p>
            <p class="text-xs text-forest-300">Cagayan State University - Carig Campus</p>
          </div>
          <div class="bg-forest-900/40 p-6 rounded-xl border border-forest-800/60 space-y-2">
            <h2 class="text-xs uppercase tracking-widest font-semibold text-gold-accent">
              High School Honors
            </h2>
            <p class="font-bold text-cream-bg">Tuao Vocational & Technical School</p>
            <p class="text-xs text-forest-300">Graduated with Honors | Best in Work Immersion</p>
          </div>
        </div>

        <!-- Certificates & Achievements -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div class="bg-forest-900/40 p-6 rounded-xl border border-forest-800/60 space-y-2">
            <h2 class="text-xs uppercase tracking-widest font-semibold text-gold-accent">
              Certificates
            </h2>
            <p class="font-semibold text-cream-bg">Civil Service Eligibility</p>
            <p class="text-xs text-forest-300">
              Professional Level Passer, Civil Service Commission (2025)
            </p>
          </div>
          <div class="bg-forest-900/40 p-6 rounded-xl border border-forest-800/60 space-y-2">
            <h2 class="text-xs uppercase tracking-widest font-semibold text-gold-accent">
              Achievements
            </h2>
            <p class="font-semibold text-cream-bg">Excellence in Practical Training</p>
            <p class="text-xs text-forest-300">Best in Work Immersion Award</p>
          </div>
        </div>

        <!-- Contact & Location Info -->
        <div
          class="grid grid-cols-1 md:grid-cols-2 gap-6 pt-6 border-t border-forest-800/80 text-sm"
        >
          <div class="bg-forest-900/40 p-5 rounded-xl border border-forest-800/60 space-y-2.5">
            <h2 class="text-xs uppercase tracking-widest font-semibold text-gold-accent">
              Contact Information
            </h2>
            <p class="flex items-center gap-2.5 text-forest-200"><span>📞</span> 099-2385-2016</p>
            <p class="flex items-center gap-2.5 text-forest-200">
              <span>✉️</span> paddananmecaella4@gmail.com
            </p>
            <p class="flex items-center gap-2.5 text-forest-200">
              <span>🔗</span>
              <a
                href="https://github.com/NotSoCuteElla"
                target="_blank"
                class="text-gold-accent hover:underline"
                >GitHub Profile</a
              >
            </p>
          </div>

          <div class="bg-forest-900/40 p-5 rounded-xl border border-forest-800/60 space-y-2.5">
            <h2 class="text-xs uppercase tracking-widest font-semibold text-gold-accent">
              Location
            </h2>
            <div class="flex items-start gap-2.5">
              <span class="text-gold-accent text-base">📍</span>
              <div>
                <p class="font-medium text-cream-bg">Tuao East, Cagayan Valley, Philippines</p>
                <p class="text-xs text-forest-300 mt-0.5">
                  Open for remote & on-site opportunities
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

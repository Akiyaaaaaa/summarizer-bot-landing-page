<script setup>
const githubUrl = 'https://github.com/Akiyaaaaaa/summary-discord-bot';
</script>
<template>
  <nav
    class="fixed top-0 left-0 right-0 z-50 backdrop-blur-md bg-[rgba(19,19,20,0.8)] border-b border-white/5 transition-all"
  >
    <div
      class="max-w-[1400px] mx-auto px-6 h-16 flex justify-between items-center"
    >
      <div class="flex items-center gap-3">
        <span class="text-2xl">✨</span>
        <span
          class="font-medium text-[1.1rem] tracking-tight text-(--text-primary)"
          >AI Summarizer</span
        >
      </div>
      <div class="flex items-center gap-6">
        <a
          :href="githubUrl"
          target="_blank"
          rel="noopener noreferrer"
          class="hidden sm:inline-block text-(--text-secondary) hover:text-white transition-colors text-sm font-medium"
        >
          GitHub
        </a>
        <a
          href="#invite"
          class="bg-(--accent-blue) hover:bg-(--accent-blue-hover) text-[#0e0e0e] px-5 py-2 rounded-full text-sm font-medium transition-colors"
        >
          Get started
        </a>
      </div>
    </div>
  </nav>
</template>

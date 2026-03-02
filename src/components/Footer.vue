<script setup>
const githubUrl = 'https://github.com/Akiyaaaaaa/summary-discord-bot';
</script>
<template>
  <footer class="bg-(--bg-color) py-12 px-6">
    <div
      class="max-w-[1400px] mx-auto flex flex-col md:flex-row justify-between items-center gap-6"
    >
      <div class="flex items-center gap-3">
        <span class="text-xl">✨</span>
        <span class="font-medium text-white text-[1.05rem]">AI Summarizer</span>
      </div>

      <div
        class="text-(--text-secondary) text-sm inline-flex flex-wrap justify-center gap-x-6 gap-y-2"
      >
        <p>&copy; {{ new Date().getFullYear() }} Akiyaaaaaa.</p>
        <a
          href="https://opensource.org/licenses/MIT"
          target="_blank"
          rel="noopener noreferrer"
          class="hover:text-white transition-colors"
          >MIT License</a
        >
        <a
          :href="githubUrl"
          target="_blank"
          rel="noopener noreferrer"
          class="hover:text-white transition-colors"
          >Source Code</a
        >
      </div>
    </div>
  </footer>
</template>

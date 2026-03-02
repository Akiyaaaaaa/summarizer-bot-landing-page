<script setup>
const githubUrl = 'https://github.com/Akiyaaaaaa/summary-discord-bot';
</script>
<template>
  <header class="relative pt-32 pb-24 lg:pt-48 lg:pb-32 px-6 overflow-hidden">
    <div
      class="absolute top-[-20%] left-0 w-full h-[600px] fire-bg opacity-35 blur-[120px] pointer-events-none mix-blend-screen"
    ></div>

    <div class="max-w-4xl mx-auto text-center space-y-8 relative z-10">
      <h1
        class="text-5xl sm:text-7xl lg:text-[5.5rem] font-semibold tracking-tight leading-[1.1] text-white"
      >
        Do more with your <br />
        <span class="text-transparent bg-clip-text bg-(--gemini-gradient)"
          >Discord community</span
        >
      </h1>
      <p
        class="text-[1.25rem] sm:text-[1.5rem] text-(--text-secondary) max-w-2xl mx-auto font-normal leading-relaxed"
      >
        Unlock the power of Gemini AI right inside your server. Summarize long
        chats, check the vibe, and keep up with ease.
      </p>

      <div
        class="pt-6 flex flex-col sm:flex-row items-center justify-center gap-4"
      >
        <a
          href="#invite"
          class="w-full sm:w-auto px-8 py-4 bg-(--accent-blue) hover:bg-(--accent-blue-hover) text-[#0e0e0e] text-[1.05rem] font-medium rounded-full transition-all flex items-center justify-center gap-2"
        >
          Add to Discord
        </a>
        <a
          :href="githubUrl"
          target="_blank"
          rel="noopener noreferrer"
          class="w-full sm:w-auto px-8 py-4 bg-transparent hover:bg-white/5 text-(--accent-blue) text-[1.05rem] font-medium rounded-full transition-all border border-white/10 flex items-center justify-center"
        >
          View Source Code
        </a>
      </div>
    </div>
  </header>
</template>

<style scoped>
.fire-bg {
  background: linear-gradient(90deg, #ff4e50, #f9d423, #ff4e50);
  background-size: 200% 100%;
  animation: move-bg 8s linear infinite;
}

@keyframes move-bg {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: -200% 50%;
  }
}
</style>

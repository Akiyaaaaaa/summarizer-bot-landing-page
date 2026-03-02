<script setup>
const steps = [
  {
    id: 1,
    title: 'Invite the Bot',
    description: 'Add the summarizer to your server with a single click.',
  },
  {
    id: 2,
    title: 'Command the AI',
    description: 'Use /summarize or other slash commands in any text channel.',
  },
  {
    id: 3,
    title: 'Get Insights',
    description:
      'Receive beautiful, intelligent summaries and insights instantly.',
  },
];
</script>
<template>
  <div
    class="relative max-w-[1400px] mx-auto my-12 sm:mx-8 rounded-[3rem] p-[2px] bg-(image:--gemini-gradient) hover:shadow-[0_0_40px_rgba(155,114,203,0.3)] transition-shadow duration-500"
  >
    <section
      class="relative bg-[#181a1b] rounded-[calc(3rem-2px)] px-6 py-24 sm:py-32 overflow-hidden w-full h-full"
    >
      <div
        class="absolute top-0 left-0 w-[500px] h-[500px] bg-linear-to-br from-[#d96570] to-[#fbbc04] opacity-[0.22] blur-[120px] rounded-full pointer-events-none mix-blend-screen -translate-x-1/4 -translate-y-1/4"
      ></div>

      <div class="text-center mb-16 md:mb-24 relative z-10">
        <h2
          class="text-4xl sm:text-5xl font-semibold mb-6 text-white tracking-tight"
        >
          How to get started
        </h2>
      </div>

      <div
        class="grid md:grid-cols-3 gap-12 lg:gap-8 max-w-5xl mx-auto relative z-10"
      >
        <div
          v-for="step in steps"
          :key="step.id"
          class="flex flex-col items-center text-center group"
        >
          <div
            class="w-20 h-20 rounded-full bg-(--bg-color) border border-white/10 flex items-center justify-center text-[2rem] font-medium text-(--accent-blue) mb-8 shadow-sm group-hover:scale-110 group-hover:border-(--accent-blue) transition-all duration-300"
          >
            {{ step.id }}
          </div>
          <h3 class="text-[1.5rem] font-medium mb-3 text-white tracking-tight">
            {{ step.title }}
          </h3>
          <p
            class="text-(--text-secondary) text-[1.1rem] leading-relaxed max-w-xs"
          >
            {{ step.description }}
          </p>
        </div>
      </div>
    </section>
  </div>
</template>

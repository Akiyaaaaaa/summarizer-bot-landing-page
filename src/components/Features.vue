<script setup>
const features = [
  {
    icon: '📝',
    title: 'Summarization',
    description: 'Get concise bullet-point summaries of recent chat history.',
    highlight: false,
  },
  {
    icon: '🕐',
    title: 'Catch-Up',
    description: 'Missed the conversation? Quick recap of the last N hours.',
    highlight: false,
  },
  {
    icon: '✅',
    title: 'Action Items',
    description: 'Automatically extract to-dos and tasks from the chat.',
    highlight: false,
  },
  {
    icon: '🌡️',
    title: 'Vibe Check',
    description: 'Analyze the mood and sentiment of a chat in real-time.',
    highlight: false,
  },
  {
    icon: '⚡',
    title: 'Gemini Powered',
    description:
      "Leverages Google's latest AI models for lightning-fast, accurate responses.",
    highlight: true,
  },
  {
    icon: '🔥',
    title: 'Roasting',
    description: 'Get a playful, AI-generated roast based on chat messages.',
    highlight: false,
  },
];
</script>

<template>
  <section class="relative max-w-[1400px] mx-auto px-6 py-24">
    <div
      class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[800px] h-[800px] bg-(--accent-blue) opacity-30 blur-[150px] rounded-full pointer-events-none mix-blend-screen"
    ></div>

    <div class="text-center mb-16 md:mb-24 relative z-10">
      <h2
        class="text-4xl sm:text-5xl font-semibold mb-6 text-white tracking-tight"
      >
        Everything you need
      </h2>
      <p class="text-(--text-secondary) text-[1.25rem] max-w-2xl mx-auto">
        Built from the ground up to make managing active servers effortless.
      </p>
    </div>

    <div
      class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 relative z-10"
    >
      <div
        v-for="(feature, index) in features"
        :key="index"
        class="relative rounded-3xl p-[2px] transition-all duration-500 group h-full"
        :class="
          feature.highlight
            ? 'bg-(image:--gemini-gradient) shadow-[0_0_30px_rgba(168,199,250,0.15)]'
            : 'bg-white/5 hover:bg-(image:--gemini-gradient) hover:shadow-[0_0_30px_rgba(155,114,203,0.25)]'
        "
      >
        <div
          class="relative h-full w-full overflow-hidden bg-(--bg-surface) rounded-[calc(1.5rem-2px)] p-8 sm:p-10 transition-colors group-hover:bg-[#181a1b]"
          :class="{
            'bg-linear-to-br from-(--bg-surface) to-[#1a2333]':
              feature.highlight,
          }"
        >
          <div
            v-if="feature.highlight"
            class="absolute top-0 right-0 w-32 h-32 bg-(--accent-blue) rounded-full blur-[80px] opacity-10 pointer-events-none"
          ></div>

          <div
            class="text-4xl mb-8 inline-block transition-transform duration-300 group-hover:scale-110 group-hover:-translate-y-1"
          >
            {{ feature.icon }}
          </div>

          <h3 class="text-[1.35rem] font-medium mb-3 text-white tracking-tight">
            {{ feature.title }}
          </h3>
          <p class="text-(--text-secondary) leading-relaxed text-[1.05rem]">
            {{ feature.description }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

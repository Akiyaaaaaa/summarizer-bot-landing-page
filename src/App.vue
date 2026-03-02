<script setup>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Features from './components/Features.vue';
import HowItWorks from './components/HowItWorks.vue';
import Cta from './components/Cta.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <div
    class="min-h-screen bg-(--bg-color) text-(--text-primary) font-sans antialiased overflow-x-hidden selection:bg-[#a8c7fa] selection:text-[#131314]"
  >
    <Navbar />
    <Hero />
    <Features />
    <HowItWorks />
    <Cta />
    <Footer />
  </div>
</template>

<style>
html {
  scroll-behavior: smooth;
}
</style>

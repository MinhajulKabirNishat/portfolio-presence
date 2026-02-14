<template>
  <div class="animate-in">
    <header class="mb-16">
      <h2 class="text-4xl font-extrabold tracking-tighter text-black mb-4">
        Selected Projects
      </h2>
      <p class="text-lg text-gray-500 max-w-2xl leading-relaxed">
        A collection of web applications and digital experiments focusing on 
        functionality, performance, and minimalistic design.
      </p>
    </header>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      <ProjectCard 
        title="ZeroHunger" 
        description="A specialized web application designed to optimize food security and distribution networks."
        link="https://github.com/MinhajulKabirNishat/ZeroHunger" 
      />

      <ProjectCard 
        title="Portfolio Presence" 
        description="A high-end digital business card built with Vue 3, Vite, and Tailwind CSS for a premium SaaS feel."
        link="https://github.com/MinhajulKabirNishat/portfolio-presence" 
      />

      <ProjectCard 
        title="nutriLife-backend" 
        description="A comprehensive diet recommendation and nutrition tracking backend system built for university. Supports three user roles: Users (clients), Dietitians, and Admins."
        link="https://github.com/MinhajulKabirNishat/nutriLife-backend.git" 
      />

      <div class="border-2 border-dashed border-gray-100 rounded-2xl p-8 flex flex-col items-center justify-center text-center opacity-50">
        <div class="h-12 w-12 bg-gray-50 rounded-full flex items-center justify-center mb-4">
          <span class="text-xl text-gray-400">+</span>
        </div>
        <p class="text-sm font-medium text-gray-400">Coming Soon</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import ProjectCard from '../components/ProjectCard.vue'
</script>

<style scoped>
.animate-in {
  animation: fadeIn 0.8s ease-out forwards;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
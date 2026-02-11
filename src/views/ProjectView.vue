<template>
  <div class="projects-page">
    <h2>My Portfolio Projects</h2>
    
    <div class="projects-grid">
      <ProjectCard 
        title="ZeroHunger" 
        description="A web application focused on food security and distribution."
        link="https://github.com/MinhajulKabirNishat/ZeroHunger" 
      />

      <ProjectCard 
        title="Portfolio Presence" 
        description="My digital business card built with Vue 3 and Vite."
        link="#" 
      />
    </div>
  </div>
</template>

<script setup>
import ProjectCard from '../components/ProjectCard.vue'
</script>

<style scoped>
.projects-page {
  padding: 40px;
  text-align: center;
}

.projects-grid {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap; 
  margin-top: 30px;
}
</style>
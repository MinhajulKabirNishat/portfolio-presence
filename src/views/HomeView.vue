<template>
  <div class="hero">
    <h1>Minhajul Kabir Nishat</h1>
    
    <p>Student & Emerging Developer</p>
    
    <div class="badge">Digital Business Card</div>
  </div>
</template>

<script setup>
// We don't need logic yet, but we keep this here for future features
</script>

<style scoped>
/* 'scoped' means these styles only affect THIS page */
.hero {
  text-align: center;
}

h1 {
  font-size: 3.5rem;
  margin-bottom: 10px;
  color: #2c3e50;
  letter-spacing: -1px;
}

p {
  font-size: 1.2rem;
  color: #666;
}

.badge {
  display: inline-block;
  margin-top: 20px;
  padding: 8px 16px;
  background-color: #42b883; 
  color: white;
  border-radius: 20px;
  font-weight: bold;
  text-transform: uppercase;
  font-size: 0.8rem;
}
</style>
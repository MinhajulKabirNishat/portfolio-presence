<template>
  <div class="card">
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
    <a :href="link" target="_blank" class="github-btn">View Code</a>
  </div>
</template>

<script setup>
defineProps(['title', 'description', 'link'])
</script>

<style scoped>
.card {
  background: white;
  border: 1px solid #eee;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.3s ease; 
  max-width: 300px;
  text-align: left;
}

.card:hover {
  transform: translateY(-10px); 
  border-color: #42b883;
}

.github-btn {
  display: inline-block;
  margin-top: 15px;
  color: #42b883;
  text-decoration: none;
  font-weight: bold;
  border: 1px solid #42b883;
  padding: 5px 12px;
  border-radius: 5px;
}

.github-btn:hover {
  background: #42b883;
  color: white;
}
</style>
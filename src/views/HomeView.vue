<template>
  <div class="hero">
    <h1>Minhajul Kabir Nishat</h1>
    <p>Student & Emerging Developer</p>
    <div class="badge">Digital Business Card</div>

    <div class="contact-box">
      <h3>Let's Connect</h3>
      <div class="social-links">
        <a href="https://github.com/MinhajulKabirNishat" target="_blank">GitHub</a>
        <a href="mailto:minhajulkabirnishat@gmail.com">Email Me</a>
      </div>
    </div>
  </div>
</template>

<script setup>
// We don't need logic yet, but we keep this here for future features
</script>

<style scoped>

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
.contact-box {
  margin-top: 50px;
  padding: 20px;
  border-top: 1px solid #eee;
}

.social-links a {
  margin: 0 15px;
  color: #2c3e50;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s;
}

.social-links a:hover {
  color: #42b883;
}
</style>
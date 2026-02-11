<template>
  <div id="app-container">
    <nav class="navbar">
      <div class="logo">MKN</div>
      <div class="links">
        <router-link to="/">Home</router-link>
        <router-link to="/projects">Projects</router-link>
      </div>
    </nav>

    <main class="content">
      <router-view />
    </main>
  </div>
</template>

<style>

body {
  margin: 0;
  font-family: 'Inter', sans-serif;
  background-color: #ffffff;
  color: #333;
}

.navbar {
  display: flex;
  justify-content: space-between;
  padding: 20px 50px;
  background: #1a1a1a;
  color: white;
}

.links a {
  color: white;
  margin-left: 20px;
  text-decoration: none;
  font-weight: bold;
}

.content {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh;
}
</style>
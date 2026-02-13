<template>
  <section class="max-w-3xl animate-in fade-in slide-in-from-bottom-8 duration-1000">
    
    <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-emerald-50 border border-emerald-100 mb-8">
      <span class="relative flex h-2 w-2">
        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
        <span class="relative inline-flex rounded-full h-2 w-2 bg-emerald-500"></span>
      </span>
      <span class="text-[10px] font-bold uppercase tracking-wider text-emerald-700">Available for new projects</span>
    </div>

    <h1 class="text-5xl md:text-7xl font-extrabold tracking-tighter text-black mb-8 leading-[1.05]">
      Crafting digital <br />
      <span class="text-gray-400">experiences that matter.</span>
    </h1>

    <p class="text-xl text-gray-500 mb-10 leading-relaxed max-w-xl">
      I'm <span class="text-black font-semibold">Minhajul Kabir Nishat</span>. 
      A developer dedicated to building clean, high-performance web applications 
      with a focus on minimalistic design and user-centric logic.
    </p>
    
    <div class="flex flex-wrap items-center gap-4">
      <router-link 
        to="/projects" 
        class="px-8 py-4 bg-black text-white rounded-2xl font-bold hover:shadow-2xl hover:shadow-black/20 hover:-translate-y-1 transition-all duration-300"
      >
        Explore Projects
      </router-link>
      
      <a 
        href="https://github.com/MinhajulKabirNishat" 
        target="_blank"
        class="px-8 py-4 border border-gray-200 rounded-2xl font-bold hover:bg-gray-50 hover:border-gray-300 transition-all duration-300 flex items-center gap-2"
      >
        <span>GitHub Profile</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M15 3h6v6"/><path d="M10 14 21 3"/><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/></svg>
      </a>
    </div>

    <div class="mt-24 pt-10 border-t border-gray-100">
      <p class="text-xs font-bold uppercase tracking-[0.2em] text-gray-400 mb-6">Expertise</p>
      <div class="flex flex-wrap gap-8 opacity-50 grayscale hover:grayscale-0 transition-all duration-500">
        <span class="font-bold text-xl tracking-tighter">Vue.js</span>
        <span class="font-bold text-xl tracking-tighter">TailwindCSS</span>
        <span class="font-bold text-xl tracking-tighter">Vite</span>
        <span class="font-bold text-xl tracking-tighter">Node.js</span>
      </div>
    </div>
  </section>
</template>

<script setup>

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
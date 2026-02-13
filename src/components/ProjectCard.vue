<template>
  <div class="group relative bg-white border border-gray-100 p-8 rounded-2xl transition-all duration-500 hover:border-gray-300 hover:shadow-2xl hover:shadow-gray-200/50">
    
    <div class="flex justify-between items-start mb-6">
      <div class="p-3 bg-gray-50 rounded-xl group-hover:bg-black group-hover:text-white transition-colors duration-300">
        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"></path></svg>
      </div>
      
      <a :href="link" target="_blank" class="text-gray-300 hover:text-black transition-colors">
        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path><polyline points="15 3 21 3 21 9"></polyline><line x1="10" y1="14" x2="21" y2="3"></line></svg>
      </a>
    </div>

    <h3 class="text-xl font-bold mb-2 tracking-tight text-black">{{ title }}</h3>
    <p class="text-gray-500 text-sm leading-relaxed mb-6">
      {{ description }}
    </p>
    
    <div class="flex items-center gap-2 text-xs font-bold uppercase tracking-widest text-gray-400 group-hover:text-black transition-colors">
      <span>View Source</span>
      <span class="transform group-hover:translate-x-1 transition-transform duration-300">→</span>
    </div>

    <div class="absolute bottom-0 left-0 h-1 bg-black w-0 group-hover:w-full transition-all duration-500"></div>
  </div>
</template>

<script setup>
defineProps(['title', 'description', 'link'])
</script>


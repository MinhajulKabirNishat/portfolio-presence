
<template>
  <div class="group relative bg-white dark:bg-zinc-900 border border-gray-100 dark:border-zinc-800 rounded-3xl overflow-hidden transition-all duration-500 hover:border-gray-300 dark:hover:border-zinc-700 hover:shadow-2xl hover:shadow-gray-200/30 dark:hover:shadow-none">
    
    <div class="relative aspect-video overflow-hidden bg-gray-100 dark:bg-zinc-800">
      <img 
        :src="image" 
        :alt="title" 
        class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-110"
      />
      
      <div class="absolute top-4 left-4 p-2.5 bg-white/90 dark:bg-zinc-900/90 backdrop-blur-md rounded-xl shadow-sm transition-colors duration-300 group-hover:bg-black group-hover:text-white">
        <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"></path></svg>
      </div>

      <a :href="link" target="_blank" class="absolute top-4 right-4 p-2 text-white bg-black/20 hover:bg-black/40 rounded-full backdrop-blur-sm transition-all">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path><polyline points="15 3 21 3 21 9"></polyline><line x1="10" y1="14" x2="21" y2="3"></line></svg>
      </a>
    </div>

    <div class="p-7">
      <h3 class="text-xl font-bold mb-2 tracking-tight text-black dark:text-white">
        {{ title }}
      </h3>
      <p class="text-gray-500 dark:text-gray-400 text-sm leading-relaxed mb-6">
        {{ description }}
      </p>
      
      <div class="flex items-center gap-2 text-[10px] font-black uppercase tracking-[0.2em] text-gray-400 dark:text-zinc-500 group-hover:text-black dark:group-hover:text-white transition-colors">
        <span>View Source</span>
        <span class="transform group-hover:translate-x-1 transition-transform duration-300">→</span>
      </div>
    </div>

    <div class="absolute bottom-0 left-0 h-1 bg-black dark:bg-white w-0 group-hover:w-full transition-all duration-500"></div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  link: String,
  image: {
    type: String,
    default: 'https://images.unsplash.com/photo-1618477388954-7852f32655ec?q=80&w=800&auto=format&fit=crop' // Placeholder
  }
})
</script>
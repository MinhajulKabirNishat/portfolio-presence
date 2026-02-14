
<template>
  <div class="min-h-screen bg-[#fafafa] dark:bg-[#0a0a0a] font-sans transition-colors duration-300">
    
    <nav class="sticky top-0 z-50 border-b border-gray-100 dark:border-zinc-800 bg-white/80 dark:bg-black/80 backdrop-blur-md">
      <div class="max-w-5xl mx-auto px-6 h-16 flex items-center justify-between">
        
        <div class="flex items-center gap-10">
          <span class="text-xl font-bold tracking-tighter text-black dark:text-white">MKN.</span>
          
          <div class="hidden md:flex gap-8 text-sm font-medium text-gray-500 dark:text-zinc-400">
            <router-link 
              to="/" 
              class="hover:text-black dark:hover:text-white transition-colors" 
              active-class="text-black dark:text-white font-semibold"
            >
              Overview
            </router-link>
            <router-link 
              to="/projects" 
              class="hover:text-black dark:hover:text-white transition-colors" 
              active-class="text-black dark:text-white font-semibold"
            >
              Projects
            </router-link>
          </div>
        </div>

        <div class="flex items-center gap-4">
          <button 
            @click="toggleDark" 
            class="p-2 rounded-xl bg-gray-100 dark:bg-zinc-800 text-gray-500 dark:text-zinc-400 hover:text-black dark:hover:text-white transition-all border border-transparent hover:border-gray-200 dark:hover:border-zinc-700"
            aria-label="Toggle Dark Mode"
          >
            <svg v-if="isDark" xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="5"/><line x1="12" y1="1" x2="12" y2="3"/><line x1="12" y1="21" x2="12" y2="23"/><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"/><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"/><line x1="1" y1="12" x2="3" y2="12"/><line x1="21" y1="12" x2="23" y2="12"/><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"/><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"/></svg>
            <svg v-else xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path></svg>
          </button>

          <a 
            href="mailto:your-email@example.com" 
            class="text-sm font-bold px-5 py-2 rounded-full bg-black dark:bg-white text-white dark:text-black hover:bg-gray-800 dark:hover:bg-zinc-200 transition-all shadow-sm"
          >
            Contact
          </a>
        </div>
      </div>
      
      <div class="md:hidden flex justify-center gap-6 pb-4 text-xs font-bold uppercase tracking-widest text-gray-500 dark:text-zinc-500">
        <router-link to="/" active-class="text-black dark:text-white">Home</router-link>
        <router-link to="/projects" active-class="text-black dark:text-white">Projects</router-link>
      </div>
    </nav>

    <main class="max-w-5xl mx-auto px-6 py-12 md:py-24">
      <router-view />
    </main>

  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const isDark = ref(false)

const toggleDark = () => {
  isDark.value = !isDark.value
  if (isDark.value) {
    document.documentElement.classList.add('dark')
    localStorage.theme = 'dark'
  } else {
    document.documentElement.classList.remove('dark')
    localStorage.theme = 'light'
  }
}


onMounted(() => {
  if (localStorage.theme === 'dark' || (!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
    isDark.value = true
    document.documentElement.classList.add('dark')
  } else {
    isDark.value = false
    document.documentElement.classList.remove('dark')
  }
})
</script>
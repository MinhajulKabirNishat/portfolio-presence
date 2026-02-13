<template>
  <div class="min-h-screen bg-[#fafafa] font-sans">
    
    <nav class="sticky top-0 z-50 border-b border-gray-100 bg-white/80 backdrop-blur-md">
      <div class="max-w-5xl mx-auto px-6 h-16 flex items-center justify-between">
        
        <div class="flex items-center gap-10">
          <span class="text-xl font-bold tracking-tighter text-black">MKN.</span>
          
          <div class="hidden md:flex gap-8 text-sm font-medium text-gray-500">
            <router-link 
              to="/" 
              class="hover:text-black transition-colors" 
              active-class="text-black font-semibold"
            >
              Overview
            </router-link>
            <router-link 
              to="/projects" 
              class="hover:text-black transition-colors" 
              active-class="text-black font-semibold"
            >
              Projects
            </router-link>
          </div>
        </div>

        <div class="flex items-center">
          <a 
            href="mailto:your-email@example.com" 
            class="text-sm font-bold px-5 py-2 rounded-full bg-black text-white hover:bg-gray-800 transition-all shadow-sm"
          >
            Contact
          </a>
        </div>
      </div>
      
      <div class="md:hidden flex justify-center gap-6 pb-4 text-xs font-bold uppercase tracking-widest text-gray-500">
        <router-link to="/" active-class="text-black">Home</router-link>
        <router-link to="/projects" active-class="text-black">Projects</router-link>
      </div>
    </nav>

    <main class="max-w-5xl mx-auto px-6 py-12 md:py-24">
      <router-view />
    </main>

  </div>
</template>




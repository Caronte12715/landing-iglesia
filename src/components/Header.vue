<template>
  <header 
    :class="[
      'fixed w-full top-0 z-50 transition-all duration-700',
      isScrolled ? 'bg-chr-secondary/95 backdrop-blur-md shadow-sm py-4' : 'bg-transparent py-6'
    ]"
  >
    <div class="max-w-7xl mx-auto px-6 flex justify-between items-center">
      <!-- Logo -->
      <a href="#" class="flex items-center gap-4 group">
        <svg class="w-8 h-8 text-chr-primary transition-transform duration-700 group-hover:scale-110" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1">
          <path d="M12 2v20M7 7h10" stroke-linecap="round"/>
        </svg>
        <span class="font-serif text-2xl tracking-[0.15em] uppercase" :class="isScrolled ? 'text-chr-dark' : 'text-chr-light'">
          Comunidad <span class="text-chr-primary font-bold">Luz</span>
        </span>
      </a>

      <!-- Desktop Nav -->
      <nav class="hidden md:flex items-center gap-10">
        <a v-for="link in links" :key="link.name" :href="link.href" 
           class="font-sans text-sm tracking-[0.2em] uppercase transition-colors duration-500 hover:text-chr-primary"
           :class="isScrolled ? 'text-chr-dark/70' : 'text-chr-light/80'">
          {{ link.name }}
        </a>
        <a href="#contacto" 
           class="px-8 py-3 border transition-all duration-500 font-sans text-sm tracking-widest uppercase"
           :class="isScrolled ? 'border-chr-dark/20 text-chr-dark hover:bg-chr-dark hover:text-chr-secondary' : 'border-chr-light/30 text-chr-light hover:bg-chr-light hover:text-chr-dark'">
          Visítanos
        </a>
      </nav>

      <!-- Mobile Button -->
      <button class="md:hidden transition-colors" :class="isScrolled ? 'text-chr-dark' : 'text-chr-light'">
        <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" stroke-width="1">
          <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16"/>
        </svg>
      </button>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const links = [
  { name: 'Inicio', href: '#' },
  { name: 'Ministerios', href: '#ministerios' },
  { name: 'Sermones', href: '#sermones' }
]

const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

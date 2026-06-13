<script setup>
import { ref, onMounted, onUnmounted } from 'vue';

const isScrolled = ref(false);
const isMobileMenuOpen = ref(false);

const handleScroll = () => {
  isScrolled.value = window.scrollY > 20;
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>

<template>
  <header 
    :class="[
      'fixed w-full top-0 z-50 transition-all duration-300',
      isScrolled ? 'bg-white shadow-md py-4' : 'bg-transparent py-6'
    ]"
  >
    <div class="max-w-7xl mx-auto px-6 flex justify-between items-center">
      <!-- Logo -->
      <a href="#" :class="[
        'text-2xl font-serif font-bold tracking-tight transition-colors duration-300',
        isScrolled ? 'text-chr-dark' : 'text-white'
      ]">
        Comunidad<span class="text-chr-primary">.</span>
      </a>

      <!-- Desktop Nav -->
      <nav class="hidden md:flex items-center gap-8">
        <a href="#reuniones" :class="['text-sm font-semibold hover:text-chr-primary transition-colors', isScrolled ? 'text-chr-dark' : 'text-white']">Reuniones</a>
        <a href="#ministerios" :class="['text-sm font-semibold hover:text-chr-primary transition-colors', isScrolled ? 'text-chr-dark' : 'text-white']">Ministerios</a>
        <a href="#nosotros" :class="['text-sm font-semibold hover:text-chr-primary transition-colors', isScrolled ? 'text-chr-dark' : 'text-white']">Nosotros</a>
        <a href="#visitar" class="bg-chr-primary hover:bg-orange-700 text-white px-6 py-2.5 rounded-full font-semibold text-sm transition-all shadow-md">
          Planear Visita
        </a>
      </nav>

      <!-- Mobile Toggle -->
      <button 
        @click="isMobileMenuOpen = !isMobileMenuOpen" 
        :class="['md:hidden p-2 transition-colors', isScrolled ? 'text-chr-dark' : 'text-white']"
      >
        <svg v-if="!isMobileMenuOpen" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
        <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </button>
    </div>

    <!-- Mobile Menu -->
    <div 
      v-if="isMobileMenuOpen" 
      class="md:hidden absolute top-full left-0 w-full bg-white shadow-xl border-t border-gray-100 flex flex-col"
    >
      <a href="#reuniones" class="p-4 border-b border-gray-50 text-center font-semibold text-chr-dark">Reuniones</a>
      <a href="#ministerios" class="p-4 border-b border-gray-50 text-center font-semibold text-chr-dark">Ministerios</a>
      <a href="#nosotros" class="p-4 border-b border-gray-50 text-center font-semibold text-chr-dark">Nosotros</a>
      <a href="#visitar" class="p-4 bg-chr-primary text-white text-center font-bold">Planear Visita</a>
    </div>
  </header>
</template>

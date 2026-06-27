<template>
  <section class="py-24 relative overflow-hidden bg-chr-dark text-chr-secondary border-y border-chr-primary/20">
    <div class="absolute inset-0 opacity-10 bg-[url('/images/church_hero.png')] bg-cover bg-center bg-fixed pointer-events-none"></div>
    <div class="absolute inset-0 bg-gradient-to-b from-chr-dark/50 to-chr-dark/90 pointer-events-none"></div>
    
    <!-- Light ray effect -->
    <div class="absolute top-0 left-1/2 -translate-x-1/2 w-full max-w-lg h-full light-ray pointer-events-none"></div>

    <div class="max-w-4xl mx-auto px-6 relative z-10 text-center reveal">
      <div class="inline-flex items-center gap-4 mb-8">
        <div class="w-12 h-px bg-chr-primary"></div>
        <span class="font-serif tracking-[0.2em] text-chr-primary uppercase text-sm">Palabra del Día</span>
        <div class="w-12 h-px bg-chr-primary"></div>
      </div>
      
      <h2 class="font-serif text-4xl md:text-5xl lg:text-6xl leading-tight mb-8 font-light italic">
        "El Señor es mi pastor, nada me falta; en verdes pastos me hace descansar. Junto a tranquilas aguas me conduce."
      </h2>
      
      <p class="font-sans tracking-widest text-chr-accent uppercase text-sm font-semibold">
        SALMO 23:1-2
      </p>
    </div>
  </section>
</template>

<script setup>
// En una implementación real, este componente podría hacer un fetch
// a una API de versículos diarios o seleccionarlo de un array según la fecha.
</script>

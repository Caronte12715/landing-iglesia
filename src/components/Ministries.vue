<template>
  <section id="ministerios" class="py-32 bg-chr-secondary relative">
    <div class="max-w-7xl mx-auto px-6">
      
      <div class="text-center mb-24 reveal">
        <span class="font-sans text-chr-primary tracking-[0.2em] uppercase text-sm mb-4 block">
          Nuestras Áreas
        </span>
        <h2 class="font-serif text-4xl md:text-5xl text-chr-dark font-light">
          Crece con <span class="italic text-chr-primary">Nosotros</span>
        </h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div v-for="(min, index) in ministries" :key="index" 
             class="group relative bg-chr-light p-10 border border-chr-dark/5 hover:border-chr-primary/30 transition-colors duration-700 reveal"
             :class="`delay-${(index + 1) * 100}`">
          
          <!-- Large Roman Numeral Background -->
          <div class="absolute -top-4 -right-4 font-serif text-8xl text-chr-secondary/80 font-bold pointer-events-none transition-transform duration-700 group-hover:-translate-y-4">
            {{ min.num }}
          </div>

          <div class="relative z-10">
            <h3 class="font-serif text-2xl text-chr-dark mb-4">{{ min.title }}</h3>
            <p class="font-sans text-chr-dark/70 font-light leading-relaxed mb-8">
              {{ min.desc }}
            </p>
            <a href="#" class="inline-flex items-center gap-2 font-sans text-sm tracking-widest uppercase text-chr-primary hover:text-chr-dark transition-colors duration-300">
              Ver detalles
              <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M17 8l4 4m0 0l-4 4m4-4H3"/></svg>
            </a>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<script setup>
const ministries = [
  {
    num: 'I',
    title: 'Adoración',
    desc: 'Únete a un equipo apasionado por guiar a la congregación hacia la presencia de Dios a través de la música y las artes.'
  },
  {
    num: 'II',
    title: 'Niños & Jóvenes',
    desc: 'Un espacio seguro y divertido donde la próxima generación puede aprender valores eternos y desarrollar su propia fe.'
  },
  {
    num: 'III',
    title: 'Obra Social',
    desc: 'Llevamos esperanza práctica a nuestra ciudad. Participa en nuestros comedores, brigadas y programas comunitarios.'
  }
]
</script>

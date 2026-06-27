<template>
  <section class="py-32 bg-chr-secondary relative">
    <div class="max-w-7xl mx-auto px-6">
      
      <div class="flex flex-col md:flex-row justify-between items-end mb-20 reveal">
        <div>
          <span class="font-sans text-chr-primary tracking-[0.2em] uppercase text-sm mb-4 block">
            Calendario
          </span>
          <h2 class="font-serif text-4xl md:text-5xl text-chr-dark font-light">
            Próximos <span class="italic text-chr-primary">Eventos</span>
          </h2>
        </div>
        <a href="#" class="mt-6 md:mt-0 font-sans text-sm tracking-widest uppercase text-chr-dark border-b border-chr-dark pb-1 hover:text-chr-primary hover:border-chr-primary transition-colors">
          Ver agenda completa
        </a>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-3 gap-10">
        <div v-for="(event, index) in events" :key="index" 
             class="group border-t border-chr-dark/10 pt-8 reveal"
             :class="`delay-${(index + 1) * 100}`">
          
          <div class="flex justify-between items-start mb-6">
            <div class="font-serif text-chr-dark">
              <span class="block text-6xl font-light leading-none group-hover:text-chr-primary transition-colors duration-500">{{ event.day }}</span>
              <span class="block text-xl tracking-widest uppercase mt-2 text-chr-accent font-semibold">{{ event.month }}</span>
            </div>
            <div class="w-12 h-12 rounded-full border border-chr-primary/30 flex items-center justify-center group-hover:bg-chr-primary group-hover:text-chr-light transition-all duration-500">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M12 4v16m8-8H4"/></svg>
            </div>
          </div>
          
          <h3 class="font-serif text-2xl text-chr-dark mb-3">{{ event.title }}</h3>
          <p class="font-sans text-chr-dark/60 font-light leading-relaxed mb-4">
            {{ event.desc }}
          </p>
          <div class="flex items-center gap-4 font-sans text-xs uppercase tracking-widest text-chr-dark/40">
            <span>{{ event.time }}</span>
            <span class="w-1 h-1 rounded-full bg-chr-primary"></span>
            <span>{{ event.location }}</span>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<script setup>
const events = [
  {
    day: '15',
    month: 'OCT',
    title: 'Noche de Adoración',
    desc: 'Una velada especial dedicada completamente a la alabanza, oración y búsqueda espiritual en comunidad.',
    time: '19:30 HRS',
    location: 'Auditorio Principal'
  },
  {
    day: '22',
    month: 'OCT',
    title: 'Bautismos',
    desc: 'Celebramos el paso de obediencia de los nuevos creyentes. Acompáñanos a testificar este hermoso acto público de fe.',
    time: '11:00 HRS',
    location: 'Campus Central'
  },
  {
    day: '05',
    month: 'NOV',
    title: 'Retiro de Jóvenes',
    desc: 'Tres días de desconexión para conectar con Dios. Conferencias, fogatas y amistades que duran para siempre.',
    time: 'TODO EL DÍA',
    location: 'Campamento Betel'
  }
]
</script>

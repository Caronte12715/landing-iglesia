<script setup>
const gatherings = [
  { day: 'Domingos', time: '10:00 AM & 12:30 PM', desc: 'Servicio General y Escuela Dominical para niños.' },
  { day: 'Miércoles', time: '7:30 PM', desc: 'Estudio Bíblico y Tiempo de Oración.' },
  { day: 'Viernes', time: '8:00 PM', desc: 'Reunión de Jóvenes (14-25 años).' }
];

const ministries = [
  { name: 'Kids', icon: '🎨', desc: 'Un ambiente seguro y divertido donde los niños aprenden valores y fe.' },
  { name: 'Jóvenes', icon: '🎸', desc: 'Música, comunidad y conversaciones relevantes para la juventud actual.' },
  { name: 'Grupos Pequeños', icon: '☕', desc: 'Conecta con otras personas durante la semana en casas o cafeterías.' },
  { name: 'Ayuda Social', icon: '🤝', desc: 'Sirviendo a nuestra ciudad entregando alimentos y amor.' }
];
</script>

<template>
  <section id="reuniones" class="py-24 bg-white relative">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-16">
      
      <!-- Horarios -->
      <div class="bg-chr-secondary p-10 md:p-14 rounded-3xl">
        <h2 class="font-serif text-3xl md:text-4xl font-bold text-chr-dark mb-8">Nuestras Reuniones</h2>
        <div class="space-y-8">
          <div v-for="(gath, index) in gatherings" :key="index" class="border-b border-chr-dark/10 pb-6 last:border-0">
            <h3 class="text-xl font-bold text-chr-primary mb-1">{{ gath.day }} <span class="text-chr-dark ml-2 text-lg">{{ gath.time }}</span></h3>
            <p class="text-gray-600">{{ gath.desc }}</p>
          </div>
        </div>
      </div>

      <!-- Ministerios -->
      <div id="ministerios">
        <div class="mb-10">
          <h2 class="font-serif text-3xl md:text-4xl font-bold text-chr-dark mb-4">Para Toda la Familia</h2>
          <p class="text-gray-600 text-lg">Tenemos un lugar especial para cada etapa de la vida. ¡Involúcrate!</p>
        </div>
        
        <div class="grid sm:grid-cols-2 gap-6">
          <div v-for="(min, index) in ministries" :key="index" class="bg-chr-light p-6 rounded-2xl border border-gray-100 shadow-sm hover:shadow-md transition-shadow group">
            <div class="text-4xl mb-4 transform group-hover:scale-110 transition-transform origin-left">{{ min.icon }}</div>
            <h3 class="text-xl font-bold text-chr-dark mb-2">{{ min.name }}</h3>
            <p class="text-gray-600 text-sm leading-relaxed">{{ min.desc }}</p>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

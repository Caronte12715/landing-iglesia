<script setup>
</script>

<template>
  <section class="relative h-screen min-h-[600px] flex items-center justify-center overflow-hidden">
    <!-- Background Image -->
    <div class="absolute inset-0 z-0">
      <img src="/images/hero.png" alt="Worship Service" class="w-full h-full object-cover object-center" />
      <div class="absolute inset-0 bg-chr-dark/50 mix-blend-multiply"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 text-center px-4 max-w-4xl mx-auto mt-16 animate-fade-in">
      <span class="text-chr-secondary font-bold tracking-widest uppercase text-sm mb-6 block drop-shadow-md">
        No importa de dónde vengas
      </span>
      <h1 class="font-serif text-5xl md:text-7xl lg:text-8xl text-white mb-8 leading-tight drop-shadow-lg">
        Bienvenido a <br/>
        <span class="text-chr-primary italic font-medium">Casa</span>
      </h1>
      <p class="text-chr-secondary text-lg md:text-xl font-light mb-12 max-w-2xl mx-auto drop-shadow-md leading-relaxed">
        Somos una comunidad apasionada por amar a Dios y servir a las personas. Queremos conocerte y caminar contigo.
      </p>
      
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <a href="#visitar" class="w-full sm:w-auto bg-chr-primary hover:bg-orange-700 text-white px-10 py-4 rounded-full font-bold transition-all shadow-xl hover:-translate-y-1">
          Planear una Visita
        </a>
        <a href="#reuniones" class="w-full sm:w-auto bg-white/10 backdrop-blur-md border border-white/30 hover:bg-white hover:text-chr-dark text-white px-10 py-4 rounded-full font-bold transition-all hover:-translate-y-1">
          Ver Horarios
        </a>
      </div>
    </div>
  </section>
</template>

<style scoped>
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
.animate-fade-in {
  animation: fadeIn 1s ease-out forwards;
}
</style>

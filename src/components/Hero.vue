<template>
  <section class="relative min-h-screen flex items-center justify-center overflow-hidden bg-chr-dark">
    <!-- Background Image with Arch Mask -->
    <div class="absolute inset-0 flex items-center justify-center pointer-events-none p-10 mt-20">
      <div class="w-full max-w-5xl h-[80vh] relative">
        <!-- Arch shape clip-path -->
        <div class="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1437603568260-1950d3ca6eab?q=80&w=2000&auto=format&fit=crop')] bg-cover bg-center opacity-40 transition-transform duration-[20s] hover:scale-105" 
             style="clip-path: polygon(0% 100%, 100% 100%, 100% 30%, 50% 0%, 0% 30%); border-radius: 50% 50% 0 0 / 20% 20% 0 0;">
        </div>
        <div class="absolute inset-0 bg-gradient-to-t from-chr-dark via-transparent to-transparent"></div>
      </div>
    </div>

    <!-- Soft Overlay -->
    <div class="absolute inset-0 bg-chr-dark/30 pointer-events-none"></div>

    <!-- Content -->
    <div class="relative z-10 text-center max-w-4xl mx-auto px-6 reveal">
      <span class="block font-sans text-chr-primary tracking-[0.3em] uppercase text-sm mb-6 opacity-90">
        Bienvenido a tu Casa
      </span>
      
      <h1 class="font-serif text-5xl md:text-7xl lg:text-8xl text-chr-light mb-8 leading-[1.1]">
        Experimenta la <br/>
        <span class="text-chr-primary italic font-light">Luz Verdadera</span>
      </h1>
      
      <p class="font-sans text-chr-accent text-lg md:text-xl max-w-2xl mx-auto mb-12 font-light leading-relaxed">
        Una comunidad unida por el propósito, la fe y el amor. Ven tal como eres y descubre tu lugar en nuestra familia espiritual.
      </p>
      
      <div class="flex flex-col sm:flex-row items-center justify-center gap-6">
        <a href="#contacto" class="bg-chr-primary text-chr-secondary px-10 py-4 font-sans tracking-widest uppercase text-sm font-semibold hover:bg-chr-light hover:text-chr-dark transition-colors duration-500 w-full sm:w-auto text-center">
          Planear Visita
        </a>
        <a href="#ministerios" class="text-chr-light px-10 py-4 font-sans tracking-widest uppercase text-sm flex items-center gap-3 hover:text-chr-primary transition-colors duration-500 group w-full sm:w-auto justify-center">
          Conocer más
          <svg class="w-4 h-4 transition-transform duration-500 group-hover:translate-x-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M17 8l4 4m0 0l-4 4m4-4H3"/></svg>
        </a>
      </div>
    </div>
  </section>
</template>

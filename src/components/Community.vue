<template>
  <section class="py-32 bg-chr-light relative overflow-hidden">
    <div class="max-w-7xl mx-auto px-6">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
        
        <div class="reveal">
          <span class="inline-block px-4 py-1 bg-chr-secondary text-chr-primary font-sans text-xs tracking-widest uppercase mb-8">
            Nuestro Impacto
          </span>
          <h2 class="font-serif text-4xl md:text-5xl text-chr-dark mb-6 leading-tight">
            Más que reuniones, <br/>
            somos <span class="text-chr-primary italic font-light">Comunidad</span>.
          </h2>
          <p class="font-sans text-chr-dark/70 text-lg leading-relaxed mb-10 max-w-lg">
            Creemos que la fe se vive en las relaciones cotidianas. Organizamos grupos pequeños, cenas comunitarias y jornadas de voluntariado donde realmente puedes conocer a otros y marcar la diferencia.
          </p>
          <a href="#" class="inline-flex items-center gap-4 bg-chr-dark text-chr-light px-8 py-4 font-sans tracking-widest uppercase text-sm font-semibold hover:bg-chr-primary transition-colors duration-500">
            Unirse a un grupo
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"/></svg>
          </a>
        </div>

        <div class="relative h-[600px] reveal delay-200">
          <!-- Mosaico Collage -->
          <div class="absolute top-0 right-0 w-2/3 h-2/3">
            <img src="/images/community.png" class="w-full h-full object-cover shadow-2xl" alt="Community gathering" />
          </div>
          <div class="absolute bottom-0 left-0 w-2/3 h-2/3 z-10 border-8 border-chr-light">
            <img src="/images/community.png" class="w-full h-full object-cover shadow-2xl" alt="Volunteering" />
          </div>
          
          <!-- Decorative element -->
          <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-32 h-32 bg-chr-primary/90 rounded-full flex items-center justify-center z-20 shadow-xl">
            <div class="text-center text-chr-dark">
              <span class="block font-serif text-3xl">50+</span>
              <span class="block font-sans text-[10px] tracking-widest uppercase font-bold">Grupos Activos</span>
            </div>
          </div>
        </div>
        
      </div>
    </div>
  </section>
</template>

<template>
  <section id="sermones" class="relative py-32 bg-chr-dark overflow-hidden border-y border-chr-primary/20">
    <!-- Parallax Background -->
    <div class="absolute inset-0 bg-[url('/images/church_hero.png')] bg-cover bg-center bg-fixed opacity-30"></div>
    <div class="absolute inset-0 bg-chr-dark/80 backdrop-blur-sm"></div>

    <div class="max-w-7xl mx-auto px-6 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
        
        <div class="reveal">
          <span class="inline-block px-4 py-1 border border-chr-primary text-chr-primary font-sans text-xs tracking-widest uppercase mb-8">
            Serie Actual
          </span>
          
          <h2 class="font-serif text-5xl md:text-6xl lg:text-7xl text-chr-light font-light mb-6">
            Tiempos de <br/> <span class="italic text-chr-primary font-bold">Esperanza</span>
          </h2>
          
          <p class="font-sans text-chr-secondary/80 text-lg leading-relaxed mb-10 max-w-md">
            En medio de la incertidumbre, encontramos un ancla segura. Únete a nuestra nueva serie de mensajes donde exploraremos las promesas eternas.
          </p>
          
          <div class="flex items-center gap-6">
            <button class="w-16 h-16 rounded-full bg-chr-primary flex items-center justify-center text-chr-dark hover:scale-110 hover:bg-chr-light transition-all duration-500 shadow-[0_0_30px_rgba(212,175,55,0.3)]">
              <svg class="w-6 h-6 ml-1" fill="currentColor" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg>
            </button>
            <span class="font-sans text-chr-light tracking-widest uppercase text-sm font-semibold">Ver último mensaje</span>
          </div>
        </div>

        <div class="relative reveal delay-200">
          <div class="aspect-square max-w-md mx-auto relative group">
            <div class="absolute inset-0 bg-gradient-to-tr from-chr-primary to-transparent opacity-20 rounded-full blur-3xl transition-opacity duration-1000 group-hover:opacity-40"></div>
            <img src="/images/sermon_cover.png" alt="Sermon Cover" class="w-full h-full object-cover rounded-t-full rounded-b-md shadow-2xl shadow-chr-dark" />
            
            <!-- Floating overlay -->
            <div class="absolute -bottom-6 -left-6 bg-chr-secondary p-6 shadow-xl border border-chr-dark/5 max-w-[200px]">
              <p class="font-serif text-chr-dark text-lg mb-1">Vol. 4</p>
              <p class="font-sans text-chr-accent text-sm uppercase tracking-widest">En vivo cada Domingo</p>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

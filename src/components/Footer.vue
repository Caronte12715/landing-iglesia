<template>
  <footer class="bg-chr-dark pt-24 pb-12 text-chr-secondary border-t border-chr-primary/20">
    <div class="max-w-7xl mx-auto px-6">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-16 mb-16 text-center md:text-left reveal">
        
        <div>
          <div class="flex items-center justify-center md:justify-start gap-4 mb-6">
            <svg class="w-6 h-6 text-chr-primary" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5">
              <path d="M12 2v20M7 7h10" stroke-linecap="round"/>
            </svg>
            <span class="font-serif text-xl tracking-widest uppercase">
              Comunidad <span class="text-chr-primary">Luz</span>
            </span>
          </div>
          <p class="font-sans text-chr-secondary/60 font-light leading-relaxed max-w-sm mx-auto md:mx-0">
            Iluminando nuestra ciudad con esperanza, fe y servicio desinteresado.
          </p>
        </div>

        <div>
          <h4 class="font-serif text-lg text-chr-primary mb-6">Reuniones</h4>
          <ul class="space-y-4 font-sans text-chr-secondary/80 font-light">
            <li>Domingos: 9:00 AM & 11:30 AM</li>
            <li>Miércoles: 7:30 PM (Estudio)</li>
            <li>Viernes: 8:00 PM (Jóvenes)</li>
          </ul>
        </div>

        <div>
          <h4 class="font-serif text-lg text-chr-primary mb-6">Ubicación</h4>
          <ul class="space-y-4 font-sans text-chr-secondary/80 font-light">
            <li>123 Avenida de la Paz</li>
            <li>Sector Central, CP 10000</li>
            <li class="mt-4"><a href="#" class="text-chr-primary hover:text-chr-light transition-colors">Ver en el mapa</a></li>
          </ul>
        </div>

      </div>

      <div class="border-t border-chr-secondary/10 pt-8 flex flex-col md:flex-row justify-between items-center gap-4 font-sans text-xs text-chr-secondary/40 uppercase tracking-widest">
        <p>&copy; {{ new Date().getFullYear() }} Comunidad Luz. Todos los derechos reservados.</p>
        <div class="flex gap-6">
          <a href="#" class="hover:text-chr-primary transition-colors">Instagram</a>
          <a href="#" class="hover:text-chr-primary transition-colors">YouTube</a>
          <a href="#" class="hover:text-chr-primary transition-colors">Facebook</a>
        </div>
      </div>
    </div>
  </footer>
</template>

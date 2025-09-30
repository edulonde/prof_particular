<template>
  <header class="fixed top-0 w-full bg-white shadow-sm z-50">
    <nav class="container mx-auto px-4 py-3">
      <div class="flex justify-between items-center">
        <div class="text-xl font-bold text-blue-800">
          Profa. Dra. Ana Silva
        </div>
        
        <!-- Mobile Menu Button -->
        <button 
          @click="toggleMenu"
          class="md:hidden p-2"
        >
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path v-if="!menuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>

        <!-- Desktop Menu -->
        <div class="hidden md:flex space-x-6">
          <a v-for="item in menuItems" :key="item.id" 
             :href="item.href" 
             class="text-gray-700 hover:text-blue-800 transition">
            {{ item.text }}
          </a>
        </div>
      </div>

      <!-- Mobile Menu -->
      <div v-if="menuOpen" class="md:hidden mt-4 pb-4">
        <a v-for="item in menuItems" :key="item.id" 
           :href="item.href" 
           @click="toggleMenu"
           class="block py-2 text-gray-700 hover:text-blue-800">
          {{ item.text }}
        </a>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      menuOpen: false,
      menuItems: [
        { id: 1, text: 'Início', href: '#hero' },
        { id: 2, text: 'Quem Sou', href: '#about' },
        { id: 3, text: 'Experiência', href: '#experience' },
        { id: 4, text: 'Serviços', href: '#services' },
        { id: 5, text: 'Apostila Grátis', href: '#ebook' }
      ]
    }
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen
    }
  }
}
</script>
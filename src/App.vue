<template>
  <div class="min-h-screen bg-white">
    <Header />
    <main>
      <Hero />
      <About />
      <Experience />
      <Services />
      <Ebook />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Experience from './components/Experience.vue'
import Services from './components/Services.vue'
import Ebook from './components/Ebook.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    About,
    Experience,
    Services,
    Ebook,
    Footer
  }
}
</script>
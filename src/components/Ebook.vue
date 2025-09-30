<template>
  <section id="ebook" class="py-16 bg-gradient-to-br from-blue-800 to-blue-600">
    <div class="container mx-auto px-4">
      <div class="max-w-4xl mx-auto text-center text-white">
        <h2 class="text-3xl md:text-4xl font-bold mb-4">
          Guia Prático para uma Redação Nota 1000
        </h2>
        <p class="text-xl mb-8 opacity-90">
          Receba gratuitamente meu material exclusivo e comece a melhorar sua redação hoje mesmo!
        </p>
        
        <div class="bg-white rounded-lg p-8 max-w-2xl mx-auto">
          <form @submit.prevent="submitForm" class="space-y-4">
            <div>
              <input 
                v-model="form.name"
                type="text" 
                placeholder="Seu nome completo" 
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
                required
              >
            </div>
            <div>
              <input 
                v-model="form.email"
                type="email" 
                placeholder="Seu melhor e-mail" 
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
                required
              >
            </div>
            <button 
              type="submit"
              class="w-full bg-blue-800 text-white py-3 rounded-lg font-semibold hover:bg-blue-900 transition"
            >
              Quero Receber a Apostila Grátis!
            </button>
          </form>
          
          <p class="text-sm text-gray-600 mt-4">
            🔒 Seu e-mail está 100% seguro. Usaremos apenas para enviar conteúdos gratuitos sobre português.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Ebook',
  data() {
    return {
      form: {
        name: '',
        email: ''
      }
    }
  },
  methods: {
    submitForm() {
      // Aqui você pode integrar com um serviço de email como Mailchimp, Google Forms, etc.
      console.log('Formulário enviado:', this.form)
      alert('Obrigada! Em breve você receberá a apostila gratuita no seu e-mail.')
      this.form.name = ''
      this.form.email = ''
    }
  }
}
</script>
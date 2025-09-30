<template>
  <section id="experience" class="py-16 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl md:text-4xl font-bold text-center text-gray-900 mb-12">
        Minha Trajetória e Qualificação
      </h2>
      
      <div class="max-w-4xl mx-auto grid md:grid-cols-2 gap-8">
        <!-- Formação Acadêmica -->
        <div class="bg-white p-6 rounded-lg shadow-sm">
          <h3 class="text-xl font-bold text-blue-800 mb-4">Formação Acadêmica</h3>
          <ul class="space-y-4">
            <li class="flex items-start">
              <span class="text-green-500 mr-3">✓</span>
              <span><strong>Doutorado em Letras</strong><br>Universidade de São Paulo (USP)</span>
            </li>
            <li class="flex items-start">
              <span class="text-green-500 mr-3">✓</span>
              <span><strong>Graduação em Letras - Português</strong><br>Universidade de São Paulo (USP)</span>
            </li>
          </ul>
        </div>
        
        <!-- Experiência Profissional -->
        <div class="bg-white p-6 rounded-lg shadow-sm">
          <h3 class="text-xl font-bold text-blue-800 mb-4">Experiência Profissional</h3>
          <ul class="space-y-4">
            <li class="flex items-start">
              <span class="text-green-500 mr-3">✓</span>
              <span><strong>Mais de 10 anos</strong> de experiência em aulas particulares</span>
            </li>
            <li class="flex items-start">
              <span class="text-green-500 mr-3">✓</span>
              <span>Preparação para <strong>ENEM, vestibulares e concursos</strong></span>
            </li>
            <li class="flex items-start">
              <span class="text-green-500 mr-3">✓</span>
              <span>Experiência em <strong>correção de redação</strong> e bancas examinadoras</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Experience'
}
</script>
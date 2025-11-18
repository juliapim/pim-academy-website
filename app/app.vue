<template>
  <div class="overflow-x-hidden min-h-screen font-sans bg-gray-50">
    <NuxtRouteAnnouncer />

    <!-- CABEÇALHO / HEADER: Identidade e Navegação (Com Logo Centralizado) -->
    <header class="bg-white shadow-lg sticky top-0 z-50">
      <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex items-center justify-between relative">
        <!-- Links Esquerda -->
        <div class="hidden sm:flex space-x-6 text-sm lg:text-base">
          <a href="#cursos" class="text-gray-700 hover:text-blue-600 font-medium transition duration-300">Cursos de Imersão</a>
          <a href="#estrutura" class="text-gray-700 hover:text-blue-600 font-medium transition duration-300">Estrutura</a>
        </div>

        <!-- LOGO CENTRALIZADO - IMAGEM DINÂMICA DA PASTA 'assets' -->
        <div class="absolute inset-0 flex justify-center items-center pointer-events-none">
          <a href="#" class="text-2xl font-extrabold pointer-events-auto flex flex-col items-center">
             <!-- Substituindo o SVG pelo logo.jpg -->
             <!-- Nota: O caminho dinâmico para assets é feito pelo Nuxt/Vite. -->
             <img src="/logo.jpg" alt="PIM Academy Logo" class="h-10 w-auto object-contain rounded-lg" onerror="this.onerror=null;this.src='https://placehold.co/100x40/467191/ffffff?text=PIM+LOGO';">
            <span class="text-xs font-medium text-gray-500 block mt-1 whitespace-nowrap">Odontologia | Cachoeiro/ES</span>
          </a>
        </div>

        <!-- Links Direita (Botão de Contato) -->
        <div class="flex space-x-6">
          <a href="#contato" style="background-color: #467191;" class="px-5 py-2 text-white rounded-full hover:opacity-90 transition duration-300 shadow-md font-medium">Fale Conosco</a>
        </div>
      </nav>
    </header>

    <!-- 1. HERO SECTION: Impacto Local e Excelência -->
    <section class="relative bg-gray-900 text-white h-[80vh] flex items-center justify-center">
      <div class="absolute inset-0 opacity-30 bg-cover bg-center" 
           style="background-image: url('https://picsum.photos/1920/1080?random=1');">
      </div>
      
      <div class="relative z-10 text-center max-w-4xl p-6">
        <h1 class="text-5xl sm:text-7xl font-extrabold leading-tight tracking-tight mb-4">
          O PÓLO DE <span class="text-blue-400">EXCELÊNCIA</span> DA ODONTOLOGIA CAPIXABA.
        </h1>
        <p class="text-xl sm:text-2xl mb-8 font-light text-gray-300">
          Imersões de Alto Nível em **Cachoeiro de Itapemirim** para transformar você em um profissional de referência.
        </p>
        <a href="#cursos" style="background-color: #467191;" class="inline-block px-10 py-4 text-xl font-bold text-white rounded-full 
                                  shadow-xl hover:opacity-90 transform hover:scale-105 transition duration-300 ease-in-out">
          Ver Próximos Cursos
        </a>
      </div>
    </section>

    <!-- 2. SEÇÃO DE CURSOS (Conversão) -->
    <section id="cursos" class="py-20 bg-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-4xl font-bold text-gray-900 mb-4">
          Cursos de Imersão Mais Procurados
        </h2>
        <p class="text-xl text-gray-600 mb-12">
          Conteúdo inovador e professores com renome nacional, agora acessível na sua região.
        </p>
        
        <!-- Grid de Cursos (Todos com o mesmo estilo: bg-gray-100, border-t-4) -->
        <div class="grid md:grid-cols-3 gap-10">
          
          <!-- Card 1: Estética (Modelo) -->
          <div class="bg-gray-100 rounded-xl shadow-lg p-6 flex flex-col items-center border-t-4 border-blue-600 hover:shadow-2xl transition duration-300">
            <div class="text-4xl text-blue-600 mb-4">🦷</div>
            <h3 class="text-2xl font-bold text-gray-900 mb-2 text-center">Imersão em Lentes de Contato Cerâmicas</h3>
            <p class="text-gray-600 text-center mb-6 flex-grow">Aprenda as técnicas mais atuais para reabilitação estética e design de sorriso.</p>
            <a href="#" style="background-color: #467191;" class="w-full py-3 text-white font-bold rounded-lg hover:opacity-90 transition duration-300 shadow-md">Saiba Mais</a>
          </div>

          <!-- Card 2: Implantodontia (Padronizado) -->
          <div class="bg-gray-100 rounded-xl shadow-lg p-6 flex flex-col items-center border-t-4 border-blue-600 hover:shadow-2xl transition duration-300">
            <div class="text-4xl text-blue-600 mb-4">🔩</div>
            <h3 class="text-2xl font-bold text-gray-900 mb-2 text-center">Cirurgia e Prótese em Implantodontia</h3>
            <p class="text-gray-600 text-center mb-6 flex-grow">Domine o planejamento e a execução de casos complexos com segurança e precisão.</p>
            <a href="#" style="background-color: #467191;" class="w-full py-3 text-white font-bold rounded-lg hover:opacity-90 transition duration-300 shadow-md">Saiba Mais</a>
          </div>
          
          <!-- Card 3: Estrutura (Padronizado para consistência, mas com conteúdo adaptado) -->
          <div id="estrutura" class="bg-gray-100 rounded-xl shadow-lg p-6 flex flex-col items-center border-t-4 border-blue-600 hover:shadow-2xl transition duration-300">
            <div class="text-4xl text-blue-600 mb-4">🏗️</div>
            <h3 class="text-2xl font-bold text-gray-900 mb-2 text-center">Nossa Estrutura de Excelência</h3>
            <p class="text-gray-600 text-center mb-6 flex-grow">Salas modernas, equipamentos de ponta e tecnologia para imersões em qualquer área do conhecimento.</p>
            <a href="#" style="background-color: #467191;" class="w-full py-3 text-white font-bold rounded-lg hover:opacity-90 transition duration-300 shadow-md">Alugue Nosso Espaço</a>
          </div>

        </div>
      </div>
    </section>
    
    <!-- 3. SEÇÃO DE FECHAMENTO (CTA e Contato) -->
    <section id="contato" class="py-20 bg-gray-900 text-white text-center">
      <div class="max-w-5xl mx-auto p-4">
        <h2 class="text-4xl sm:text-5xl font-extrabold mb-4 text-blue-400">
          Pronto para o Próximo Nível da Sua Carreira?
        </h2>
        <p class="text-xl mb-8">
          Fale diretamente com nossa equipe e garanta sua vaga nas próximas imersões.
        </p>
        <a href="https://wa.me/seunumerodecontato" target="_blank" class="inline-block px-12 py-5 text-2xl font-bold bg-green-500 text-white rounded-full 
                                  shadow-xl hover:bg-green-600 transform hover:scale-105 transition duration-300 ease-in-out">
          FALE AGORA PELO WHATSAPP
        </a>
      </div>
    </section>

    <!-- RODAPÉ (Footer) -->
    <footer class="bg-gray-800 text-white py-6">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <p class="text-gray-400">PIM.ACADEMY | Excelência em Capacitação Odontológica em Cachoeiro de Itapemirim - ES.</p>
      </div>
    </footer>
  </div>
</template>

<style>
/* Estilos globais para garantir que o Tailwind carregue corretamente */
@tailwind base;
@tailwind components;
@tailwind utilities;

/* Opcional: Efeito de rolagem suave nos links âncora */
html {
  scroll-behavior: smooth;
}
/* Cores customizadas para reuso */
.pim-blue{
  color: #467191;
}
</style>

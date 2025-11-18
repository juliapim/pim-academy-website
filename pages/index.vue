<template>
  <div class="overflow-x-hidden">
    <section class="relative bg-gray-900 text-white h-screen flex items-center justify-center">
      <div class="absolute inset-0 opacity-20 bg-cover bg-center" 
           style="background-image: url('https://picsum.photos/1920/1080?random=1');">
      </div>
      
      <div class="relative z-10 text-center max-w-4xl p-6">
        <h1 class="text-5xl sm:text-7xl font-extrabold leading-tight tracking-tight mb-4">
          <span class="text-indigo-400">LIBERDADE</span> FINANCEIRA. SEU ESCRITÓRIO É O MUNDO.
        </h1>
        <p class="text-xl sm:text-2xl mb-8 font-light text-gray-300">
          Desenvolva a habilidade digital que paga as contas e financia seus sonhos. Sem chefes, sem fronteiras.
        </p>
        <a href="#cursos" class="inline-block px-10 py-4 text-xl font-bold bg-indigo-600 text-white rounded-full 
                                  shadow-lg hover:bg-indigo-700 transform hover:scale-105 transition duration-300 ease-in-out">
          Ver Cursos e Iniciar a Jornada
        </a>
      </div>
    </section>

    <section id="cursos" class="py-20 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-4xl font-bold text-gray-900 mb-4">
          Escolha Sua Habilidade de Alto Valor
        </h2>
        <p class="text-xl text-gray-600 mb-12">
          Cursos práticos e direto ao ponto para que você comece a aplicar e gerar renda imediatamente.
        </p>
        
        <div class="grid md:grid-cols-3 gap-10">
          <CardCurso 
            titulo="Especialista em Edição de Vídeos Curtos"
            gancho="Domine a arte dos Reels e TikToks e cobre caro por isso."
            preco="R$ 997,00"
          />
          <CardCurso 
            titulo="Gestão de Mídias para Remotos"
            gancho="Gerencie perfis de marcas globais de qualquer lugar do planeta."
            preco="R$ 1.297,00"
          />
          <CardCurso 
            titulo="Freelancer PRO com IA"
            gancho="Multiplique sua produtividade e capte clientes usando ferramentas de AI."
            preco="R$ 797,00"
          />
        </div>
      </div>
    </section>
    
    <section id="sucesso" class="py-20 bg-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-4xl font-bold text-gray-900 text-center mb-12">
          Histórias de Sucesso: O Mapa da Jornada
        </h2>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-indigo-50 p-6 rounded-xl shadow-lg border-t-4 border-indigo-600">
            <p class="text-xl italic text-gray-700 mb-4">
              "Em 3 meses, recuperei o investimento e hoje estou morando na Tailândia, trabalhando apenas 4 horas por dia!"
            </p>
            <p class="font-bold text-indigo-700">- Ana P., Editora Remota</p>
          </div>
          <div class="bg-indigo-50 p-6 rounded-xl shadow-lg border-t-4 border-indigo-600">
            <p class="text-xl italic text-gray-700 mb-4">
              "O módulo de captação de clientes foi game-changer. Fechei meu primeiro contrato em dólar na primeira semana."
            </p>
            <p class="font-bold text-indigo-700">- João G., Gestor de Tráfego</p>
          </div>
          <div class="flex flex-col justify-center items-center text-center p-6 bg-gray-900 text-white rounded-xl shadow-xl">
            <h3 class="text-2xl font-bold mb-4">Seja o Próximo!</h3>
            <p class="mb-6">O sucesso não espera. Aja agora.</p>
            <a href="#cursos" class="px-8 py-3 bg-white text-indigo-600 font-bold rounded-full hover:bg-gray-200 transition">
              QUERO MINHA LIBERDADE
            </a>
          </div>
        </div>
      </div>
    </section>

    <section class="py-20 bg-indigo-600 text-white text-center">
      <div class="max-w-5xl mx-auto p-4">
        <h2 class="text-4xl sm:text-5xl font-extrabold mb-4">
          PARE DE SONHAR. COMECE A VIVER.
        </h2>
        <p class="text-xl mb-8">
          Sua vida de trabalho flexível, viagens e autonomia começa com o primeiro clique.
        </p>
        <a href="#cursos" class="inline-block px-12 py-5 text-2xl font-bold bg-white text-indigo-600 rounded-full 
                                  shadow-xl hover:bg-gray-200 transform hover:scale-105 transition duration-300 ease-in-out">
          EU QUERO ESSA VIDA!
        </a>
      </div>
    </section>
  </div>
</template>
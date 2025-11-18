<template>
  <div>
    <header class="bg-white shadow-md sticky top-0 z-50">
      <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
        <NuxtLink to="/" class="text-2xl font-bold text-indigo-600">
          PIM.ACADEMY
        </NuxtLink>
        <div class="space-x-4">
          <NuxtLink to="#cursos" class="text-gray-600 hover:text-indigo-600 font-medium transition duration-300">Cursos</NuxtLink>
          <NuxtLink to="#sucesso" class="text-gray-600 hover:text-indigo-600 font-medium transition duration-300">Histórias de Sucesso</NuxtLink>
          <a href="#" class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700 transition duration-300 shadow-md">Comece Agora</a>
        </div>
      </nav>
    </header>

    <slot />

    <footer class="bg-gray-900 text-white py-12 mt-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <p class="text-gray-400">© {{ new Date().getFullYear() }} PIM.ACADEMY. Todos os direitos reservados.</p>
        <div class="mt-4 space-x-4">
          </div>
      </div>
    </footer>
  </div>
</template>
<script setup lang="ts">
// Define as propriedades (props) que o componente CardCurso irá receber
defineProps({
  titulo: {
    type: String,
    required: true,
  },
  gancho: {
    type: String,
    required: true,
  },
  preco: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="bg-white rounded-xl shadow-2xl p-6 flex flex-col items-center transform hover:scale-[1.03] transition duration-500 border-b-8 border-indigo-500">
    <div class="text-5xl text-indigo-600 mb-4">
      🚀
    </div>
    
    <h3 class="text-2xl font-bold text-gray-900 mb-2 text-center">{{ titulo }}</h3>
    
    <p class="text-gray-600 text-center mb-6 flex-grow">{{ gancho }}</p>
    
    <div class="text-3xl font-extrabold text-indigo-600 mb-6">{{ preco }}</div>
    
    <button class="w-full py-3 bg-indigo-600 text-white font-bold rounded-lg hover:bg-indigo-700 transition duration-300 shadow-lg">
      Matricule-se Agora
    </button>
  </div>
</template>
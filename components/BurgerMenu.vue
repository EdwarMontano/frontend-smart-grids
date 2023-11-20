<template>
    <div class="px-8">
        <button @click="isOpen = !isOpen" class="lg:hidden block text-gray-500 hover:text-gray-700 focus:outline-none">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path strokeLinecap="round" strokeLinejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"
                    v-if="!isOpen"></path>
                <path strokeLinecap="round" strokeLinejoin="round" stroke-width="2" d="M6 18L18 6" v-else></path>
            </svg>
        </button>

        <div v-show="isOpen"
            class="lg:hidden bg-gray-600 absolute top-0 left-0 right-0 p-4 mt-16 z-10 border-b border-gray-200">
            <!-- Coloca aquí tus enlaces de navegación -->
            <ul class="flex space-x-2 md:space-x-4">
                    <li><a href="/description" class="text-white hover:text-gray-300 text-sm md:text-base">Descripción</a></li>
                    <li><a href="/analysis" class="text-white hover:text-gray-300 text-sm md:text-base">Análisis</a></li>
                    <li><a href="/results" class="text-white hover:text-gray-300 text-sm md:text-base">Resultados</a></li>
            </ul>
        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            isOpen: false,
        };
    },
};
</script>
  
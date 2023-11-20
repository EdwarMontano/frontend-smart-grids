<template>
    <header class="bg-gray-800 py-4">
        <div class="container mx-auto flex pl-4 justify-between items-center flex-wr ">
            <a href="/" class="flex items-center flex-shrink-0 text-white mr-6ap  border-4 rounded-md px-2 py-4 bg-white">
                <img src="/assets/logo.jpg" alt="Logo" class="h-8 w-auto md:h-10 md:w-auto ">
            </a>
            <h1 class="text-white text-xl font-bold pl-4 md:text-2xl my-2 md:my-0 sm:block  hidden">Proyecto de Redes Inteligentes</h1>
            <nav class="sm:block  hidden">
                <ul class="flex space-x-2 md:space-x-4">
                    <li><a href="/description" class="text-white hover:text-gray-300 text-sm md:text-base">Descripción</a></li>
                    <li><a href="/analysis" class="text-white hover:text-gray-300 text-sm md:text-base">Análisis</a></li>
                    <li><a href="/results" class="text-white hover:text-gray-300 text-sm md:text-base">Resultados</a></li>
                </ul>
            </nav>
            <BurgerMenu />
        </div>
    </header>
</template>

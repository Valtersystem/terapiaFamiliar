<script setup>
import Formacoes from '@/Components/Formacoes.vue'
</script>


<template>
  <section class="text-black bg-gray-50 rounded-2xl">
    <div class="mx-auto max-w-screen-xl px-4 py-8 sm:px-6 sm:py-12 lg:px-8 lg:py-16 ">
      <div class="mx-auto max-w-lg text-center">
        <h2 class="text-3xl font-bold sm:text-4xl">Formações</h2>

        <p class="mt-4 text-black">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequuntur aliquam doloribus
          nesciunt eos fugiat. Vitae aperiam fugit consequuntur saepe laborum.
        </p>
      </div>

      <div class="mt-8 grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3">
        <Formacoes />
        <Formacoes />
        <Formacoes />
        <Formacoes />
        <Formacoes />
        <Formacoes />
      </div>

      <div class="mt-12 text-center">
        <a href="#"
          class="inline-block rounded bg-white px-12 py-3 text-sm font-medium text-blue-600 border border-solid border-blue-600 transition hover:bg-blue-600 hover:text-white focus:outline-none focus:ring focus:ring-yellow-400">
          Ver mais
        </a>
      </div>
    </div>
  </section>
</template>
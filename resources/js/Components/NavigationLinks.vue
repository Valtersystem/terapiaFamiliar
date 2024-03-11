<script setup>
import NavLink from '@/Components/NavLink.vue';
</script>

<template>
  <ul
    class="flex flex-col font-medium p-4 md:p-0 mt-4 border border-gray-100 rounded-lg bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white">

    <li>
      <NavLink class="block py-2 px-3 text-gray-900 rounded" :href="route('home')" :active="route().current('home')">Home
      </NavLink>
    </li>

    <li>
      <NavLink class="block py-2 px-3 text-gray-900 rounded" :href="route('terapeutas')" :active="route().current('terapeutas')">Terapeutas
      </NavLink>
    </li>

    <li>
      <NavLink class="block py-2 px-3 text-gray-900 rounded" :href="route('formacao')" :active="route().current('formacao')">Formação
      </NavLink>
    </li>

    <li>
      <NavLink class="block py-2 px-3 text-gray-900 rounded" :href="route('biblioteca')" :active="route().current('biblioteca')">Biblioteca
      </NavLink>
    </li>

    <li>
      <NavLink class="block py-2 px-3 text-gray-900 rounded" :href="route('eventos')" :active="route().current('eventos')">Eventos
      </NavLink>
    </li>

    <li>
      <NavLink class="block py-2 px-3 text-gray-900 rounded" :href="route('contactos')" :active="route().current('contactos')">Contactos
      </NavLink>
    </li>

  </ul>
</template>
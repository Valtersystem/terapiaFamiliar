<script setup>
import NavigationLinks from '@/Components/NavigationLinks.vue';
</script>

<template>
    <nav class="bg-white border-gray-200 fixed z-50 w-full">
        <div class="flex flex-wrap items-center justify-between mx-auto p-8">
            <a href="#" class="flex items-center space-x-3 rtl:space-x-reverse">
                <img src="https://res.cloudinary.com/dtf70ty3b/image/upload/v1710109923/terapia/logo.png" class=" h-20" alt="Logo" />
            </a>
            <button data-collapse-toggle="navbar-multi-level" type="button"
                class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200"
                aria-controls="navbar-multi-level" aria-expanded="false">
                <span class="sr-only">Open main menu</span>
                <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none"
                    viewBox="0 0 17 14">
                    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M1 1h15M1 7h15M1 13h15" />
                </svg>
            </button>
            <div class="hidden w-full md:block md:w-auto" id="navbar-multi-level">
                <NavigationLinks />
            </div>
        </div>
    </nav>
</template>
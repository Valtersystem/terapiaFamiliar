<script setup>
import { ref } from 'vue';
import { Link } from '@inertiajs/vue3';
import Nav from '@/Components/Nav.vue';
</script>

<template>
    <div class="max-w-screen-[2000px] my-0 mx-auto">
        <div class="min-h-screen bg-gray-100">
            <!-- Nav Bar -->
            <Nav />

            <!-- Page Heading -->
            <header class="bg-white shadow" v-if="$slots.header">
                <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
                    <slot name="header" />
                </div>
            </header>

            <!-- Page Content -->
            <main>
                <slot />
            </main>
        </div>
    </div>
</template>

<template>
  <div class="min-h-screen bg-gradient-to-br from-indigo-50 via-white to-slate-50 text-slate-900">
    <header class="max-w-6xl mx-auto px-4 py-6 flex flex-col md:flex-row md:items-center md:justify-between gap-4">
      <div>
        <h1 class="text-2xl md:text-3xl font-bold tracking-tight">PrimeVue + Tailwind Demo</h1>
        <p class="text-sm text-slate-600 mt-1">
          Um pequeno e-commerce construído com Vue 3, PrimeVue e Tailwind CSS.
        </p>
      </div>

      <nav class="flex gap-3">
        <RouterLink
          class="rounded-lg px-4 py-2 text-sm font-medium text-slate-700 hover:bg-indigo-50 hover:text-indigo-700"
          to="/"
          >Loja</RouterLink
        >
        <RouterLink
          class="rounded-lg px-4 py-2 text-sm font-medium text-slate-700 hover:bg-indigo-50 hover:text-indigo-700"
          to="/about"
          >Sobre</RouterLink
        >
      </nav>
    </header>

    <main class="max-w-6xl mx-auto px-4 pb-12">
      <RouterView />
    </main>
  </div>
</template>

<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

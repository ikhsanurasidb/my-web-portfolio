<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="py-4 bg-gray-100 border-b-2 shadow-md">
    <nav class="flex items-center justify-center">
      <RouterLink
        to="/"
        class="ml-16 font-serif text-4xl font-semibold tracking-widest transition duration-300 ease-in-out filter drop-shadow-md hover:text-gray-400 hover:drop-shadow-2xl"
      >
        Ikhsan<span class="text-blue-400">.</span>
      </RouterLink>

      <!-- <div class="flex gap-8 mr-16">
        <a
          href="#about"
          class="text-xl font-semibold transition duration-300 ease-in-out hover:text-gray-400 filter hover:drop-shadow-2xl drop-shadow-md"
        >
          About
        </a>
        <a
          href="#projects"
          class="text-xl font-semibold transition duration-300 ease-in-out hover:text-gray-400 filter hover:drop-shadow-2xl drop-shadow-md"
        >
          Projects
        </a>
        <a
          href="#contact"
          class="text-xl font-semibold transition duration-300 ease-in-out hover:text-gray-400 filter hover:drop-shadow-2xl drop-shadow-md"
        >
          Contact
        </a>
        <a
          href="#social-media"
          class="text-xl font-semibold transition duration-300 ease-in-out hover:text-gray-400 filter hover:drop-shadow-2xl drop-shadow-md"
        >
          Social Media
        </a>
      </div> -->
    </nav>
  </header>

  <main class="min-h-screen p-6 bg-gray-100">
    <RouterView />
  </main>
</template>

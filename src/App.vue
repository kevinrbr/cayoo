<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="absolute z-1000 container mx-auto">
      <nav class="flex gap-[74px] text-white font-inter">
        <RouterLink to="/">A Propos</RouterLink>
        <RouterLink to="/">Nos loueurs</RouterLink>
        <RouterLink to="/">Contact</RouterLink>
        <RouterLink to="/">Aide</RouterLink>
      </nav>
  </header>

  <RouterView />
</template>

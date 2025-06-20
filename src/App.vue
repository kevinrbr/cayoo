<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import { Button } from '@/components/ui/button';
</script>

<template>
  <header class="absolute z-50 w-full top-0">
    <div class="container mx-auto flex items-center justify-between py-4">
      <div class="flex items-center gap-24">
        <RouterLink to="/" class="text-4xl font-bold text-primary font-satoshi">
          cayoo
        </RouterLink>

        <nav class="flex items-center gap-10 text-white font-inter mt-2">
          <RouterLink to="/">A propos</RouterLink>

          <div class="flex items-center gap-10">
            <RouterLink to="/">Nos loueurs</RouterLink>
            <RouterLink to="/">Contact</RouterLink>
            <RouterLink to="/">Aide</RouterLink>
          </div>
        </nav>
      </div>
      <div class="flex items-center gap-8">
        <RouterLink to="/" class="text-white">Connexion</RouterLink>
        <Button variant="outline" size='lg'>
          Inscription
        </Button>
      </div>
    </div>
  </header>

  <RouterView />
</template>

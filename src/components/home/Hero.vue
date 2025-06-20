<script setup lang="ts">
import InputSearch from '@/components/home/InputSearch.vue';

</script>

<template>
  <section class="!w-full fixed-width h-dvh bg-[url(/src/assets/images/home-background.jpg)] bg-cover bg-center bg-no-repeat flex flex-col justify-end">
    <div class="w-full h-full bg-black/45 absolute top-0 left-0 z-0 pointer-events-none"></div>

    <div class="relative container !mx-auto mb-28">
      <h1 class="text-white text-5xl font-bold max-w-4xl font-satoshi">
        Recherchez, louez et explorez l’Albanie à votre rythme
      </h1>
      <p class="text-white mt-6 mb-10">
        Des loueurs de confiance, soigneusement sélectionnés pour vous garantir un voyage en toute sérénité.
      </p>
      <InputSearch />
    </div>
  </section>
</template>

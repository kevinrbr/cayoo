<script setup lang="ts">
import { ref } from 'vue';
import { Button } from '@/components/ui/button';
import { Search } from 'lucide-vue-next'

const location = ref<string>('');
const fromDate = ref<string>('');
const toDate = ref<string>('');
const arrivalHour = ref<string>('9h00');
const departureHour = ref<string>('18h00');
</script>

<template>
  <div class="bg-white rounded-lg flex h-16 items-center pl-6 p-2 max-w-5xl">
    <div class="flex-1 flex items-center gap-4">
      
      <div class="flex flex-col flex-1">
        <!-- <label class="text-dark-gray text-xs" for="location">Lieu de prise en charge</label> -->
        <input class="text-sm text-black placeholder-neutral-gray w-full outline-none" v-model="location" id="location" placeholder="Aeroport, gare, ville"/>
      </div>

      <div class="flex flex-col border-l border-gray-300 pl-4 max-w-[120px]">
        <label class="text-dark-gray text-xs" for="fromDate">Arrivée</label>
        <input class="text-sm text-black placeholder-neutral-gray w-full outline-none" v-model="fromDate" id="fromDate" placeholder="De quand ?"/>
      </div>

      <div class="flex flex-col border-l border-gray-300 pl-4 max-w-[120px]">
        <label class="text-dark-gray text-xs" for="toDate">Départ</label>
        <input class="text-sm text-black placeholder-neutral-gray w-full outline-none" v-model="toDate" id="toDate" placeholder="A quand ?"/>
      </div>

      <div class="flex flex-col border-l border-gray-300 pl-4 max-w-[120px]">
        <label class="text-dark-gray text-xs" for="arrivalHour">Arrivée</label>
        <input class="text-sm text-black placeholder-neutral-gray w-full outline-none" v-model="arrivalHour" id="arrivalHour" placeholder="9h00"/>
      </div>

      <div class="flex flex-col border-l border-gray-300 pl-4 max-w-[120px]">
        <label class="text-dark-gray text-xs" for="departureHour">Départ</label>
        <input class="text-sm text-black placeholder-neutral-gray w-full outline-none" v-model="departureHour" id="departureHour" placeholder="18h00"/>
      </div>
    </div>

    <Button size="icon" class="h-full w-12 ml-4">
      <Search class="w-5 h-5"/>
    </Button>
  </div>
</template>

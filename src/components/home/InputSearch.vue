<script setup lang="ts">
import { ref } from 'vue';

const location = ref<string>('');
</script>

<template>
    <div class="bg-white rounded-lg flex h-16 items-center p-6">
        <div class="flex flex-col">
            <label class="text-dark-gray text-xs" for="location">Lieu de prise en charge</label>
            <input class="text-sm text-neutral-gray" v-model="location" id="location" placeholder="Aeroport, gare, ville"/>
        </div>
        <div class="flex flex-col">
            <label class="text-dark-gray text-xs" for="from">Arrivée</label>
            <input class="text-sm text-neutral-gray" v-model="location" id="to" placeholder="Aeroport, gare, ville"/>
        </div>
        <div class="flex flex-col">
            <label class="text-dark-gray text-xs" for="to">Départ</label>
            <input class="text-sm text-neutral-gray" v-model="location" id="to" placeholder="Aeroport, gare, ville"/>
        </div>
        <div class="flex flex-col">
            <label class="text-dark-gray text-xs" for="from">Arrivée</label>
            <input class="text-sm text-neutral-gray" v-model="location" id="to" placeholder="Aeroport, gare, ville"/>
        </div>
        <div class="flex flex-col">
            <label class="text-dark-gray text-xs" for="to">Départ</label>
            <input class="text-sm text-neutral-gray" v-model="location" id="to" placeholder="Aeroport, gare, ville"/>
        </div>
    </div>
</template>
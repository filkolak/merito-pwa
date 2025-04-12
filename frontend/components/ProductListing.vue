<template>
    <div
        class="bg-[#2b2b2b] flex border border-[#3a3a3a] rounded-md text-white shadow-sm hover:shadow-md transition-shadow duration-200 cursor-pointer p-3 w-full max-w-screen-xl">
        <img :src="image" alt="Nazwa produktu" class="w-48 h-48 object-contain mb-3 rounded" loading="lazy" />

        <div class="flex-1 ml-4">
            <div class="text-sm font-medium mb-1 line-clamp-2">
                {{ name }}
            </div>
        </div>

        <div class="text-right min-w-[100px]">
            <div class="text-lg font-bold text-green-400">
                {{ price }} zł
            </div>

            <div class="text-xs text-gray-400 mt-1">
                {{ delivery }}
            </div>

            <button class="w-full py-2 mt-2 bg-orange-500 text-white rounded-md hover:bg-orange-600 focus:outline-none">
                DODAJ DO KOSZYKA
            </button>

            <!-- Ikona serduszka po prawej stronie -->
            <button
                class="w-full py-2 mt-2 bg-gray-700 text-white rounded-md hover:bg-gray-800 focus:outline-none flex items-center justify-center">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 ml-2">
                    <path
                        d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z" />
                </svg>
            </button>
        </div>
    </div>
</template>

<script setup lang="ts">
defineProps<{
    image: string
    name: string
    price: string | number
    delivery: string
}>()
</script>
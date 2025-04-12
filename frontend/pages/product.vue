<template>
    <!-- Sekcja z tłem #222 -->
    <section class="bg-[#222222] py-6 px-4">
        <!-- Kontener wyśrodkowany -->
        <div class="max-w-screen-xl mx-auto">
            <!-- Tytuł -->
            <h2 class="text-white text-xl font-semibold mb-4">Title: {{ title }}</h2>

            <div class="flex">
                <!-- Pierwszy div (60%) po lewej stronie -->
                <div class="w-3/5 bg-[#2b2b2b] p-4 mr-4">
                    <!-- Treść pierwszego div -->
                    <img :src="image" alt="Nazwa produktu" class="w-48 h-48 object-contain mb-3 rounded"
                        loading="lazy" />
                </div>

                <!-- Drugi div (40%) po prawej stronie -->
                <div class="w-2/5 bg-[#2b2b2b] p-4">
                    <!-- Treść drugiego div -->
                    <p>Treść drugiego div</p>
                </div>
            </div>

            <!-- Trzeci div (60%) pod pierwszym z marginesem -->
            <div class="w-3/5 bg-[#2b2b2b] p-4 mt-4 mr-4">
                <!-- Treść trzeciego div -->
                <p>Treść trzeciego div</p>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
</script>
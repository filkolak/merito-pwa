<template>
    <!-- Sekcja z tłem #222 -->
    <section class="bg-[#222222] py-6 px-4">
      <!-- Kontener wyśrodkowany -->
      <div class="max-w-screen-xl mx-auto">
        <!-- Tytuł -->
        <h2 class="text-white text-xl font-semibold mb-4">{{ title }}</h2>
  
        <!-- Produkty w gridzie -->
        <div class="grid">
          <ProductListing
              v-for="(product, index) in products"
              :key="index"
              :image="product.image"
              :name="product.name"
              :price="product.price"
              :delivery="product.delivery"
          />
        </div>
      </div>
    </section>
  </template>
  
  <script setup lang="ts">
  import ProductListing from './ProductListing.vue'
  
  defineProps<{
    title: string
    products: {
      image: string
      name: string
      price: string | number
      delivery: string
    }[]
  }>()
  </script>
  
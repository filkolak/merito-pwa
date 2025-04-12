<script setup lang="ts">
// 📦 Pobieramy dane z API Nuxta (endpoint: /api/products)
const { data, pending, error } = await useFetch('/api/products')

// 🔁 Tworzymy zmienną reaktywną zawierającą tylko produkty1
const produkty1 = computed(() => data.value?.produkty1 || [])
</script>

<template>
  <BasicSlider />

  <NuxtLink to="/product">
    <ListingSection title="Listing" :products="produkty1" />
  </NuxtLink>
</template>

<style scoped></style>
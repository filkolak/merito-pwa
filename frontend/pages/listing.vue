<script setup lang="ts">
// 📦 Pobieramy dane z API Nuxta (endpoint: /api/products)
const { data, pending, error } = await useFetch('/api/products')

// 🔁 Tworzymy zmienną reaktywną zawierającą tylko produkty1
const produkty1 = computed(() => data.value?.produkty1 || [])
</script>

<template>
  <BasicSlider />

  <ListingSection title="Listing" :products="produkty1" />
</template>

<style scoped></style>
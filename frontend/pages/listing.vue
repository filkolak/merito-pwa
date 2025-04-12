<script setup lang="ts">
const produkty1 = [
  { image: 'https://picsum.photos/seed/blender/180/180', name: 'Blender KitchenMix 2000', price: '368,89', delivery: 'we wtorek' },
  { image: 'https://picsum.photos/seed/koszyk/180/180', name: 'Koszyk wielkanocny z kwiatami', price: '65,00', delivery: 'we wtorek' },
  { image: 'https://picsum.photos/seed/baby/180/180', name: 'Ochraniacz dla dzieci CARIBOO', price: '79,90', delivery: 'w środę' },
  { image: 'https://picsum.photos/seed/kosmetyki/180/180', name: 'Zestaw kosmetyków pielęgnacyjnych', price: '278,00', delivery: 'w poniedziałek' },
  { image: 'https://picsum.photos/seed/grill/180/180', name: 'Grill ogrodowy RUSZTY', price: '329,00', delivery: 'we wtorek' },
]
</script>

<template>    
      <BasicSlider/>

      <ListingSection title="Listing" :products="produkty1" />
</template>

<style scoped>
</style>
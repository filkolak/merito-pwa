<template>
  <div data-atr="tenDiv">
    <NuxtRouteAnnouncer />
    <Navbar/>
    <NuxtLayout>
      <NuxtPage/>
    </NuxtLayout>
    <FooterArticles />
    <FooterMain />
  </div>
</template>
<script setup lang="ts">
useHead({
  link: [
    { rel: 'manifest', href: '/manifest.webmanifest' }
  ]
})
</script>
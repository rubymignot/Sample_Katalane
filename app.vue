<template>
  <div>
    <NuxtPage/>
  </div>
</template>
<script setup lang="ts">
const ogImg = "/og-image.png"
useSeoMeta({
  ogImage: ogImg,
  twitterImage: ogImg,
})
useHead({
  meta: [
    { name: "twitter:image:src", content:ogImg }
  ]
})
</script>
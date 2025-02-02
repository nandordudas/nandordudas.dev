<script setup lang="ts">
import { en } from '@nuxt/ui/locale'

useHead({
  htmlAttrs: {
    lang: 'en',
    dir: 'ltr',
  },
})
</script>

<template>
  <NuxtRouteAnnouncer />
  <NuxtLoadingIndicator />

  <UApp :locale="en">
    <NuxtLayout>
      <NuxtPage :page-key="route => route.fullPath" />
    </NuxtLayout>
  </UApp>
</template>

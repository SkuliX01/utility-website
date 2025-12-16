<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

const title = "SkuliX Utility website"
const description = "Ultimate ulitty website."

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
})
</script>

<template>
  <UApp>
    <UHeader>
      <template #left>
        <NuxtLink to="/" class="flex items-center justify-center flex-row space-x-2">
          <img src="https://i.ibb.co/8Dj6m6L4/129431960.png" height="50" width="50"
            class="hidden md:block rounded-2xl"></img>
          <p class="font-bold">SkuliX Ultimate Utility</p>
        </NuxtLink>
      </template>

      <template #right>
        <UColorModeButton />

      </template>
    </UHeader>

    <UMain>
      <NuxtPage />
    </UMain>

    <USeparator />

    <UFooter>
      <template #default>
        <p class="text-sm text-muted text-center">
          Built with ❤️ by <a href="https://github.com/SkuliX01" class="underline">SkuliX</a>
        </p>
      </template>
    </UFooter>
  </UApp>
</template>

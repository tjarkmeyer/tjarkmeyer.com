<template>
  <header class="bg-white fixed max-w-5xl w-full z-10">
    <nav class="flex items-center gap-x-6 p-6">
      <div>
        <a href="/#" class="text-3xl md:text-4xl font-bold">Tjark Meyer</a>
      </div>
      <div class="hidden sm:flex sm:gap-x-12 ml-auto">
        <NuxtLink
          v-for="item in navigation"
          :key="item.name"
          :href="item.href"
          class="text-lg font-semibold leading-6 hover:text-gray-700"
          >{{ item.name }}</NuxtLink
        >
      </div>
      <GeneralBtn class="ml-auto sm:ml-6 text-lg" href="/#contact"
        >Contact</GeneralBtn
      >
    </nav>
  </header>
</template>

<script setup>
const navigation = [
  { name: 'About me', href: '/#about' },
  { name: 'Tech Stack', href: '/#techstack' },
]
</script>

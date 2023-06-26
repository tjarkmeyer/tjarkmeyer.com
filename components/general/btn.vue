<template>
  <NuxtLink
    :href="href"
    rel="noopener noreferrer"
    class="shadow-xl relative inline-flex items-center justify-start inline-block px-3 py-2 md:px-5 md:py-3 overflow-hidden font-medium transition-all bg-black rounded-3xl hover:bg-white group"
  >
    <span
      class="absolute inset-0 border-0 group-hover:border-[25px] ease-linear duration-150 transition-all border-white rounded-3xl"
    ></span>
    <span
      class="relative w-full text-left text-white transition-colors duration-150 ease-in-out group-hover:text-black"
      ><slot></slot
    ></span>
  </NuxtLink>
</template>

<script setup>
defineProps({
  href: {
    type: String,
    default: '',
  },
})
</script>

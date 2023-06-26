<template>
  <AppContainer>
    <div
      class="font-bold space-y-2 opacity-0 transition-all duration-1000 -translate-x-full"
      :class="{ 'opacity-100 translate-x-0': show }"
    >
      <div class="text-5xl">Hi 👋</div>
      <div class="text-4xl">I'm Tjark</div>
      <div class="text-2xl max-w-xl">
        Fullstack Engineer, Tech Nerd (from Vacuum Cleaners to HiFi Audio),
        Passionate Vegan
      </div>
      <div class="pt-6">
        <AppSocial></AppSocial>
      </div>
    </div>
    <ArrowDownIcon
      class="h-12 w-12 hidden sm:block absolute bottom-2 left-1/2 -translate-x-1/2 animate-bounce"
    ></ArrowDownIcon>
  </AppContainer>
</template>

<script setup lang="ts">
import { ArrowDownIcon } from '@heroicons/vue/20/solid'

const show = ref(false)
onMounted(() => (show.value = true))
</script>

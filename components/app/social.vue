<template>
  <div class="flex gap-2 md:gap-6">
    <GeneralBtn href="https://www.linkedin.com/in/tjark-meyer/">
      <svg
        fill="currentColor"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 50 50"
        width="50px"
        height="50px"
        class="w-6 h-6 sm:inline mx-auto sm:mx-0"
      >
        <path
          d="M41,4H9C6.24,4,4,6.24,4,9v32c0,2.76,2.24,5,5,5h32c2.76,0,5-2.24,5-5V9C46,6.24,43.76,4,41,4z M17,20v19h-6V20H17z M11,14.47c0-1.4,1.2-2.47,3-2.47s2.93,1.07,3,2.47c0,1.4-1.12,2.53-3,2.53C12.2,17,11,15.87,11,14.47z M39,39h-6c0,0,0-9.26,0-10 c0-2-1-4-3.5-4.04h-0.08C27,24.96,26,27.02,26,29c0,0.91,0,10,0,10h-6V20h6v2.56c0,0,1.93-2.56,5.81-2.56 c3.97,0,7.19,2.73,7.19,8.26V39z"
        ></path>
      </svg>
      LinkedIn
    </GeneralBtn>
    <GeneralBtn href="https://github.com/tjarkmeyer">
      <svg
        aria-hidden="true"
        height="24"
        viewBox="0 0 16 16"
        version="1.1"
        width="24"
        data-view-component="true"
        fill="currentColor"
        class="w-6 h-6 sm:inline mx-auto sm:mx-0"
      >
        <path
          d="M8 0c4.42 0 8 3.58 8 8a8.013 8.013 0 0 1-5.45 7.59c-.4.08-.55-.17-.55-.38 0-.27.01-1.13.01-2.2 0-.75-.25-1.23-.54-1.48 1.78-.2 3.65-.88 3.65-3.95 0-.88-.31-1.59-.82-2.15.08-.2.36-1.02-.08-2.12 0 0-.67-.22-2.2.82-.64-.18-1.32-.27-2-.27-.68 0-1.36.09-2 .27-1.53-1.03-2.2-.82-2.2-.82-.44 1.1-.16 1.92-.08 2.12-.51.56-.82 1.28-.82 2.15 0 3.06 1.86 3.75 3.64 3.95-.23.2-.44.55-.51 1.07-.46.21-1.61.55-2.33-.66-.15-.24-.6-.83-1.23-.82-.67.01-.27.38.01.53.34.19.73.9.82 1.13.16.45.68 1.31 2.69.94 0 .67.01 1.3.01 1.49 0 .21-.15.45-.55.38A7.995 7.995 0 0 1 0 8c0-4.42 3.58-8 8-8Z"
        ></path>
      </svg>
      GitHub
    </GeneralBtn>
    <GeneralBtn href="mailto:hello@tjarkmeyer.com">
      <EnvelopeIcon class="h-6 sm:inline mx-auto sm:mx-0"></EnvelopeIcon> E-Mail
    </GeneralBtn>
  </div>
</template>

<script setup lang="ts">
import { EnvelopeIcon } from '@heroicons/vue/20/solid'
</script>

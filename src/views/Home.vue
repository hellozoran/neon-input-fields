<script setup>
import InputTextarea from '../components/InputTextarea.vue'
import InputText from '../components/InputText.vue'
import { inject } from 'vue'
const $api = inject('$api')
</script>

<template>
  <section class="grid min-h-screen place-content-center relative">
    <div class="w-80">
      <img src="/neon-inputs.png" class="absolute top-1 w-40 left-3" />
      <a href="https://zoranmitrovic.com" class="text-slate-400 absolute top-8 text-sm right-6 flex items-center gap-1">
        Read the article
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
        </svg>
      </a>
      <InputText type="text" label="Your name" placeholder="Enter your name" required />
      <InputTextarea label="Text area" placeholder="Enter your message" class="mt-6" />
    </div>
  </section>
</template>
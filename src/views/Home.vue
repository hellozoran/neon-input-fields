<script setup>
import InputTextarea from '../components/InputTextarea.vue'
import InputText from '../components/InputText.vue'
import { inject } from 'vue'
const $api = inject('$api')
</script>

<template>
  <section class="grid min-h-screen place-content-center">
    <div class="w-80 space-y-6">
      <InputText type="text" label="Your name" placeholder="Enter your name" required />
      <InputTextarea label="Text area" />
    </div>
  </section>
</template>
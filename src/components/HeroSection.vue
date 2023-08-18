<script setup lang="ts"></script>

<template>
  <div class="relative overflow-hidden py-24 pl-48">
    <div class="absolute inset-0 bg-cover bg-[url('../assets/background.png')] bg-center"></div>
    <div class="relative flex items-center justify-center min-h-screen px-4 py-16 sm:py-32">
      <div class="flex flex-col items-start max-w-3xl">
        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6 text-[#292A29]">
          Run your <span class="text-[#11453B]">payroll</span>
          <span class="text-[#B4A572]"> easily</span> in <span class="text-[#EA4E4B]">seconds</span>
        </h1>
        <p class="text-xl mb-6 text-[#515251]">
          We’ve built an all-inclusive simple solution for individual and businesses to manage
          staff, pay salaries, bills, and relevant taxes all at once.
        </p>
        <div class="space-x-4 mb-[72px]">
          <button class="bg-[#11453B] hover:bg-[#11453B]/90 text-white px-9 py-4 rounded-[32px]">
            Start Using Free, Forever
          </button>
        </div>
        <div class="space-y-4 flex flex-col">
          <p class="font-medium text-lg">Download the Eazipay App</p>
          <div class="flex justify-start">
            <button>
              <img src="../assets/app-store.png" alt="app store button" class="" />
            </button>
            <button>
              <img src="../assets/google-store.png" alt="google store button" class="" />
            </button>
          </div>
        </div>
      </div>
      <div class="hidden md:block relative right-[-20px] ml-8">
        <img src="../assets/hero-image.png" alt="Hero Image" class="" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {}
})
</script>

<style scoped>
/* Add your global styles here */
</style>

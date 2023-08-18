<template>
  <nav
    class="flex w-full absolute z-10 font-medium justify-between items-center px-48 py-5 bg-transparent"
  >
    <div class="flex flex-1 items-center gap-[70px]">
      <img src="../assets/logo.png" alt="logo" class="" />
      <div class="flex justify-center items-center gap-12 text-[#515251]">
        <RouterLink to="/home" class="hover:text-gray-300">Individual</RouterLink>
        <RouterLink to="/about" class="hover:text-gray-300">Business</RouterLink>
        <RouterLink to="/services" class="hover:text-gray-300">Pricing</RouterLink>
        <RouterLink to="/contact" class="hover:text-gray-300">Set your payroll</RouterLink>
      </div>
      <!-- <div class="text-lg font-semibold">Your Logo</div> -->
    </div>

    <div class="space-x-4 text-sm">
      <button
        @click="login"
        class="bg-transparent hover:bg-[#11453B] hover:text-white border border-[#11453B] text-[#11453B] px-16 py-[10px] rounded-3xl"
      >
        Log In
      </button>
      <button
        @click="register"
        class="hover:bg-[#11453B]/95 bg-[#11453B] border border-[#11453B] hover:border-[#11453B] hover:text-white text-white px-16 py-[10px] rounded-3xl"
      >
        Register
      </button>
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { RouterLink, RouterView } from 'vue-router'

export default defineComponent({
  methods: {
    login() {},
    register() {}
  }
})
</script>

<template>
  <div class="flex flex-row items-center w-full text-gray-400 font-bold">
    <div class="flex mr-4  hover:text-gray-800 cursor-pointer">
      <router-link :to="{ name: 'home' }"> Home </router-link>
    </div>
    <div class="flex mr-4  hover:text-gray-800 cursor-pointer">
      <router-link :to="{ name: 'about' }"> About </router-link>
    </div>
    <div class="flex hover:text-gray-800 cursor-pointer">Something</div>
  </div>
</template>

<script setup lang="ts">
import { RouterLink } from "vue-router";
</script>

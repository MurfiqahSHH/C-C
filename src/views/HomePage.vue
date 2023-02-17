<template>
  <LayoutWrapper>
    <div class="flex flex-row w-full justify-around">
      <div class="flex h-20 bg-red-400">123</div>
      <div class="flex h-20 bg-blue-500">123</div>
      <div class="flex h-20 bg-green-600">123</div>
      <div class="flex h-20 bg-yellow-300">123</div>
    </div>
  </LayoutWrapper>
</template>

<script setup lang="ts">
import LayoutWrapper from "@/components/Layout/LayoutWrapper.vue";

const shownColor = "someth";
</script>

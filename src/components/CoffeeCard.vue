<template>
  <div class="flex flex-col p-4 rounded-lg bg-white shadow-lg max-w-[105px]">
    <div class="flex flex-row h-20"><img :src="data.image" alt="" class="w-full"></div>
    <div class="flex flex-row">{{data.name}}</div>
    <div class="flex flex-row">{{data.description}}</div>
    <div class="flex flex-row">{{priceFormat}}</div>
  </div>
</template>

<script setup lang="ts">
import {computed} from 'vue'
const props = defineProps({
  data: {
    type: Object
  },
});

const priceFormat = computed(() => {
  let input = props.data.price
  return '$' + input
})
</script>

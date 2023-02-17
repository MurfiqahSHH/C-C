<template>
  <div class="flex flex-col p-4 rounded-lg bg-white shadow-lg">
    <div class="flex flex-row"><img src="" alt=""></div>
    <div class="flex flex-row">Title</div>
    <div class="flex flex-row">Description</div>
    <div class="flex flex-row">price</div>
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  item: {
    type: Object
  },
});
</script>

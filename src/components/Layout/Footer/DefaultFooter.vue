<template>
  <div class="flex flex-col mt-auto bg-slate-700">
    <div class="flex flex-row p-4">
      <div class="flex flex-col">
        <div class="font-semibold text-gray-200">Title</div>
        <div class="font-light text-gray-100">Link</div>
        <div class="font-light text-gray-100">Link</div>
        <div class="font-light text-gray-100">Link</div>
        <div class="font-light text-gray-100">Link</div>
      </div>
    </div>
    <div class="flex flex-col p-4 bg-slate-800">
        <div class="flex flex-row">
            <SocialMediaLinks/>
        </div>
        <div class="flex flex-row"></div>
    </div>
  </div>
</template>

<script setup lang="ts">
import SocialMediaLinks from '@/components/SocialMediaLinks.vue';

</script>

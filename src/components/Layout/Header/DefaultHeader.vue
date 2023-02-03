<template>
    <div class="flex flex-row w-full h-20 bg-green-500">
        <div class="flex w-1/12 bg-blue-300">Logo</div>
        <div class="flex grow bg-blue-400 p-4">
            <NavBar />
        </div>
        <div class="flex w-3/12 bg-blue-300"></div>
    </div>
</template>

<script setup lang="ts">
import NavBar from '@/components/NavBar.vue';


const something = 123

</script>
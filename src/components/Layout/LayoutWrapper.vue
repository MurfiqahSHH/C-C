<template>
    <div class="flex flex-col min-w-screen min-h-screen">
        <DefaultHeader />
        <slot></slot>
        <DefaultFooter />
    </div>

    
    

</template>

<script setup lang="ts">
import DefaultFooter from './Footer/DefaultFooter.vue';
import DefaultHeader from './Header/DefaultHeader.vue'
</script>
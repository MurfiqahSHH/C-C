<template>
    <div class="flex flex-row w-full h-20 bg-white">
        <div class="flex w-1/12 ">
            <img src="src/assets/logo2.svg" alt="" class="object-contain">
        </div>
        <div class="flex grow p-4">
            <NavBar />
        </div>
        <div class="flex flex-row items-center justify-around w-3/12  text-gray-400 font-bold">
            <div class=" hover:text-gray-800 cursor-pointer" @click="toggleLoginModal">Login</div>
            <div class=" hover:text-gray-800 cursor-pointer">Sign up</div>
        </div>
    </div>
    <BaseModal 
    v-if="showLoginModal" 
    title="Login"
    @close-modal="toggleLoginModal"></BaseModal>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import BaseModal from '@/components/BaseModal.vue';
import NavBar from '@/components/NavBar.vue';


const showLoginModal = ref(false)

const toggleLoginModal = () => {
    showLoginModal.value = !showLoginModal.value
}

</script>
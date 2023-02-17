<template>
    <div class="flex flex-row w-full h-20 bg-green-500">
        <div class="flex w-1/12 bg-blue-300">Logo</div>
        <div class="flex grow bg-blue-400 p-4">
            <NavBar />
        </div>
        <div class="flex flex-row items-center justify-around w-3/12 bg-blue-300">
            <div class="ccButton" @click="toggleLoginModal">Login</div>
            <div class="ccButton">Sign up</div>
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
<template>
    <div class="flex flex-row items-center w-full text-gray-800">
                <div class="flex mr-4">
                    <router-link 
                    :to="{name : 'home'}"
                    >
                        Home
                    </router-link>
                </div>
                <div class="flex mr-4">
                    <router-link :to="{name : 'about'}">
                        About
                    </router-link>
                </div>
                <div class="flex">Something</div>
            </div>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router';



</script>
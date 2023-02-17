<template>
    <div class="absolute top-0 z-10 flex flex-col justify-center item-center  min-h-screen w-full bg-gray-400">
        <div class=" flex flex-col  self-center min-w-[50%] max-w-[75%] bg-white p-4">
            <div class="flex flex-row items-center justify-between px-2">
                <div class="text-green-600">{{title}}</div>
                <Close class=" cursor-pointer" @click="closeModal"/>
            </div>
            <div class="flex flex-row p-2">
                <slot></slot>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import Close from '@carbon/icons-vue/es/close--outline/16';
const emit = defineEmits(['close-modal', 'something-else'])
const props = defineProps({
    title: {
        type : String
    },
    modalActive : {
        type: Boolean,
        default: false
    }
})

const closeModal = () => {
    emit('close-modal', 123456)
} 

</script>
<template>
  <LayoutWrapper>
    <div class="flex flex-row">
      <CoffeeCard 
      class="mr-4"
      v-for="(coffee, index) in data" 
      :key="coffee.id"
      :data="coffee"
      />
    </div>

    <div v-if="newdata == null" class="flex flex-row mt-8">
      <template v-for="(coffee, index) in data">
        <CoffeeCard 

      :data="coffee"
      />
      </template>
    </div>
  </LayoutWrapper>
</template>

<script setup lang="ts">
import { ref, onMounted } from "vue";
import CoffeeCard from "@/components/CoffeeCard.vue";
import LayoutWrapper from "@/components/Layout/LayoutWrapper.vue";
let newdata = ref(null)

onMounted(async () => {
  const apiRes = await fetch('https://jsonplaceholder.typicode.com/users')
  newdata.value = apiRes
})

const data = [
  {
    id: 55,
    name: "coffee1",
    price: 5.99,
    description: "This is coffee 1",
    image: "https://via.placeholder.com/150",
  },
  {
    id: 56,
    name: "coffee2",
    price: 7.99,
    description: "This is coffee 2",
    image: "https://via.placeholder.com/200",
  },
  {
    id: 57,
    name: "coffee3",
    price: 8.99,
    description: "This is coffee 1",
    image: "https://via.placeholder.com/100",
  },
];
</script>

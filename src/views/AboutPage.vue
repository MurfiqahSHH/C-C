<template>
  <LayoutWrapper>
    <div class="flex flex-row">
      <CoffeeCard />
      {{ data }}
    </div>
  </LayoutWrapper>
</template>

<script setup lang="ts">
import CoffeeCard from "@/components/CoffeeCard.vue";
import LayoutWrapper from "@/components/Layout/LayoutWrapper.vue";

const data = [
  {
    name: "coffee1",
    price: 5.99,
    description: "This is coffee 1",
    image: "https://www.fillmurray.com/640/360",
  },
  {
    name: "coffee2",
    price: 7.99,
    description: "This is coffee 2",
    image: "https://www.fillmurray.com/640/700",
  },
  {
    name: "coffee3",
    price: 8.99,
    description: "This is coffee 1",
    image: "https://www.fillmurray.com/640/400",
  },
];
</script>

<script setup lang="ts">
import SneakerCartItem from './SneakerCartItem.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <div class="flex items-center gap-5">
      <img
        src="/arrow-next-cart.svg"
        alt="next arrow"
        class="opacity-30 cursor-pointer rotate-180 hover:opacity-100 transition hover:-translate-x-1"
      />
      <h2 class="text-2xl font-bold">Cart</h2>
    </div>

    <SneakerCartItem />
    <SneakerCartItem />
    <SneakerCartItem />
  </div>
</template>

<script setup>
import SneakerCardList from './components/SneakerCardList.vue'
import SneakerHeader from './components/SneakerHeader.vue'
</script>

<template>
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <SneakerHeader />

    <div class="m-10">
      <h2 class="font-bold text-3xl mb-8">All sneakers</h2>
      <SneakerCardList />
    </div>
  </div>
</template>

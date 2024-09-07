<script setup>
import SneakerCard from './SneakerCard.vue'
const onClickAdd = () => {
  console.log('Add')
}
const onClickFavorite = () => {
  console.log('Favorite')
}
</script>
<template>
  <div class="grid grid-cols-4 gap-5">
    <SneakerCard
      image-url="/sneakers/sneakers-1.jpg"
      title="Men's sneakers Nike Blazer Mid Suede"
      :price="6500"
      :is-favorite="true"
      :is-added="true"
      @click-add="onClickAdd"
      @click-favorite="onClickFavorite"
    />
  </div>
</template>

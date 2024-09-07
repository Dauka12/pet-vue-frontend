<script setup>
import SneakerCard from './SneakerCard.vue'

const onClickAdd = () => {
  console.log('clicked add in sneaker card with id:' + onClickAdd.id)
}
const onClickFavorite = () => {
  console.log('clicked favorite in sneaker card with id:' + onClickFavorite.id)
}
</script>
<template>
  <div class="grid grid-cols-4 gap-5">
    <SneakerCard
      image-url="/sneakers/sneakers-1.jpg"
      title="Men's sneakers Nike Blazer Mid Suede"
      :price="6500"
      @click-add="onClickAdd"
      @click-favorite="onClickFavorite"
      :id="17"
    />
    <SneakerCard
      image-url="/sneakers/sneakers-1.jpg"
      title="Men's sneakers Nike Blazer Mid Suede"
      :price="6500"
      @click-add="onClickAdd"
      @click-favorite="onClickFavorite"
      :id="18"
    />
  </div>
</template>

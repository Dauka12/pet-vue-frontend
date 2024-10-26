<script setup>
import { ref } from 'vue'

defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  id: Number
})
const emit = defineEmits(['click-add', 'click-favorite'])

const isAdded = ref(false)
const isFavorite = ref(false)

const onClickAdd = () => {
  isAdded.value = !isAdded.value
  emit('click-add')
}
const onClickFavorite = () => {
  isFavorite.value = !isFavorite.value
  emit('click-favorite')
}
</script>

<template>
  <div
    class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer hover:-translate-y-2 hover:shadow-xl transition"
  >
    <img
      @click="onClickFavorite"
      :src="!isFavorite ? '/like-1.svg' : '/like-2.svg'"
      alt="Like 1"
      class="absolute top-8 left-8"
    />
    <img :src="imageUrl" alt="Sneakers" />
    <p class="mt-5">{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Price:</span>
        <b>{{ price }} KZT</b>
        <span>Учу алгоритмы</span>   
      </div>
      <img @click="onClickAdd" :src="!isAdded ? '/plus.svg' : '/checked.svg'" alt="Plus" />
    </div>
  </div>
</template>

<template>
  <header class="flex justify-between border-b border-slate-200 px-10 py-8">
    <div class="flex items-center gap-4">
      <img src="/logo.png" alt="Logo" class="w-10" />
      <div>
        <h2 class="text-xl font-bold uppercase">Vue Sneakers</h2>
        <p class="text-slate-400">Best sneakers store</p>
      </div>
    </div>
    <ul class="flex gap-10 items-center">
      <li class="flex gap-3 items-center text-gray-500 hover:text-black cursor-pointer">
        <img src="/cart.svg" alt="Cart" />
        <b>8300 KZT</b>
      </li>

      <li class="flex gap-3 items-center text-gray-500 hover:text-black cursor-pointer">
        <img src="/heart.svg" alt="Heart" />
        <span>bookmarks</span>
      </li>

      <li class="flex gap-3 items-center text-gray-500 hover:text-black cursor-pointer">
        <img src="/profile.svg" alt="Heart" />
        <span>Profile</span>
      </li>
    </ul>
  </header>
</template>

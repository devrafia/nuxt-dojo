<script setup>
    const { product } = defineProps(['product']);
</script>

<template>
  <div class="flex gap-4 container">
    <div class="container w-1/2 p-4">
        <img :src="product.image" alt="product image" class="w-full rounded">    
    </div>
    <div class="flex flex-col gap-4 w-full p-4">
        <h1 class="font-bold text-xl tracking-wide">{{ product.title }}</h1>
        <span class="font-bold text-4xl">${{ product.price }}</span>
        <p class="mt-4 tracking-tight text-justify">{{ product.description }}</p>
    </div>
  </div>
</template>

<style>

</style>
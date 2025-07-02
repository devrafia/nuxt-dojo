<script setup>

    const { product } = defineProps(['product']);
</script>

<template>
  <div>
    <div class="bg-white p-4 rounded shadow-md">
      <img :src="product.image" alt="Product Image" class="w-auto h-60 mt-2 mx-auto rounded">
      <h2 class="text-xl font-bold truncate">{{ product.title }}</h2>
      <p class="text-gray-500 truncate first-letter:uppercase">{{ product.category }}</p>
      <p class="text-green-600 font-semibold">${{ product.price }}</p>
      <NuxtLink :to="`/products/${product.id}`" class="block bg-green-400 hover:bg-green-500 active:bg-green-600
      transition duration-200 p-2 w-full mt-2 rounded-lg
      text-white font-semibold cursor-pointer text-center">
        View Details
      </NuxtLink>
    </div>
  </div>
</template>


<style>

</style>
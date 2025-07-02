<script setup>
    definePageMeta({
        layout: 'products'
    })

    const { data: response } = await useFetch('https://fakestoreapi.in/api/products')
    const products = computed(() => response.value?.products ?? [])
</script>

<template>
    <div>
        <div class="p-2">
            <h1 class="block bg-white text-center font-bold text-6xl mb-4 text-shadow-xs text-green-400">Available Items!</h1>
        </div>
        <div class="grid grid-cols-4 gap-4">
            <div v-for="p in products" :key="p.id" class="p-2">
                <ProductCard :product="p" />
            </div>
        </div>
    </div>
</template>

<style>

</style>
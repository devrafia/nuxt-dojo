<script setup>
    definePageMeta({
            layout: 'products'
    })
    const {id} = useRoute().params;
    const { data: response } = await useFetch(`https://fakestoreapi.in/api/products/${id}`)
    const product = computed(() => response.value?.product ?? {})
</script>

<template>
    <div>
        <ProductDetails :product="product"/>
    </div>
</template>

<style>

</style>
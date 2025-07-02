<script setup>
</script>

<template>
    <div>
        <header class="shadow-md bg-white">
            <nav class="container mx-auto flex justify-between items-center p-4">
                <NuxtLink to="/products" class="font-bold text-shadow-xs text-green-500 text-xl"><h1>Nuxt Dojo Merch</h1></NuxtLink>
            </nav>
        </header>
        <main class="shadow-md bg-white p-4 my-4">
            <div class="container mx-auto">
                <slot />
            </div>
        </main>
        <footer class="bg-white mt-4">
            <ul class=" container mx-auto justify-between items-center p-4">
                <li class="btn"><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/products">Products</NuxtLink></li>
            </ul>
        </footer>
    </div>
</template>


<style>

</style>
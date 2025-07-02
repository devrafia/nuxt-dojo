<script setup>
</script>

<template>
  <div>
    <header class="shadow-md bg-white">
      <nav class="container mx-auto flex justify-between items-center p-4">
        <h1 class="font-bold"><NuxtLink to="/">Nuxt Dojo</NuxtLink></h1>
        <ul class="flex gap-4">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <div class="container mx-auto p-4">
        <slot />
    </div>
  </div>
</template>

<style>
    .router-link-active {
        color: lime;
    }
</style>
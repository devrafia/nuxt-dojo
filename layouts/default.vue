<script setup>
</script>

<template>
  <div>
    <header>
      <nav>
        <h1><NuxtLink to="/">Nuxt Dojo</NuxtLink></h1>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
        <a href="/">Home</a>
      </nav>
    </header>
    <div>
        <slot />
    </div>
  </div>
</template>

<style>
</style>
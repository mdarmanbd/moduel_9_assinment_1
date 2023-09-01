<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <nav class="bg-green-300 flex justify-between px-4 py-1 border border-b-yellow-400">
      <div class="">
        <p class="text-blue-950 font-bold text-lg">MR BLOG</p>
      </div>
      <div class="text-blue-950 text-lg font-semibold flex space-x-5">
        <RouterLink to="/" >Home</RouterLink>
        <RouterLink to="/about" >About</RouterLink>
        <RouterLink to="/list" >List</RouterLink>
    </div>
    </nav> 
  </header>

  <RouterView />
</template>

<style scoped>

</style>

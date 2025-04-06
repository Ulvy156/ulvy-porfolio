<template>
  <nav class="lg:flex md:flex justify-between text-white p-3 border-b border-gray-500 sticky top-0 z-50 hidden">
    <h1 class="text-2xl ml-10">Ulvy</h1>
    <ul class="flex justify-evenly w-1/2">
      <li>About</li>
      <li>Skills</li>
      <li>Projects</li>
      <li>Contact</li>
    </ul> 
    
  </nav>
  <NavbarMobile />

</template>

<script lang="ts" setup>
import NavbarMobile from './NavbarMobile.vue';


</script>

<style scoped>
nav {
  background-image: var(--bg-color);

}
</style>
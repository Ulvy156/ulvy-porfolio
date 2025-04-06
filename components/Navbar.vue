<template>
  <nav class="lg:flex md:flex justify-between text-white p-3 border-b border-gray-500 backdrop-blur-md sticky top-0 z-50 hidden ">
    <h1 class="text-2xl ml-10">Ulvy</h1>
    <div class="flex justify-evenly w-1/2">
      <a href="#git-in-touch">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div> 
    
  </nav>
  <NavbarMobile />

</template>

<script lang="ts" setup>
import NavbarMobile from './NavbarMobile.vue';


</script>

<style scoped>
/* nav {
  background-image: var(--bg-color);
} */
</style>
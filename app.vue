<template>
  <Navbar/>
  <main class="w-11/12 m-auto">
    <NuxtPage />
  </main>
  <Footer />
  <el-backtop :right="60" :bottom="60" >
    <template #default>
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="m6 11l6-6l6 6M6 19l6-6l6 6"/></svg>
    </template>
  </el-backtop>
</template>

<script lang="ts" setup>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'


</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Winky+Sans:ital,wght@0,300..900;1,300..900&display=swap');
:root {
  --bg-color: linear-gradient(to right, #363636 0%, black 100%);
}
html {
  scroll-behavior: smooth;
}
body {
  background-image: var(--bg-color);
  font-family: "Winky Sans", sans-serif;
  font-optical-sizing: auto;
}
</style>
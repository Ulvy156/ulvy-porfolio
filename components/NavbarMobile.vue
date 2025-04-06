<template>
  <nav class="flex justify-between text-white p-3 border-b border-gray-500 sticky top-0 z-50 lg:hidden md:hidden">
    <h1 class="text-2xl ">Ulvy</h1>
    <svg xmlns="http://www.w3.org/2000/svg" @click="drawer = true" class="size-7" viewBox="0 0 32 32">
      <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
        d="M12 8h15M5 16h22M5 24h22M5 11l3-3l-3-3" />
    </svg>
  </nav>
  <el-drawer size="90%"  @click="drawer = false"
    style="background: var(--bg-color);color: white; font-size: 20px;" direction="ltr" 
    v-model="drawer" :with-header="true">
    <template #header>
      <div class="flex items-center gap-x-2 text-white">
        <svg xmlns="http://www.w3.org/2000/svg" class="size-9" viewBox="0 0 24 24">
              <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-width="1.5"
                d="m17 7.83l1.697 1.526c1.542 1.389 2.313 2.083 2.313 2.974c0 .89-.771 1.585-2.314 2.973L17 16.83M13.987 5L12 12.415l-1.987 7.415M7 7.83L5.304 9.356C3.76 10.745 2.99 11.44 2.99 12.33s.771 1.585 2.314 2.973L7 16.83" />
            </svg>
        <h1 class="text-3xl ">Ulvy</h1>
      </div>
    </template>
    <div class="grid grid-cols-1 gap-5 ">
      <a href="#git-in-touch">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div> 
  </el-drawer>

</template>

<script lang="ts" setup>

const drawer = ref<boolean>(false);

</script>

<style scoped>
nav {
  background-image: var(--bg-color);
}

</style>
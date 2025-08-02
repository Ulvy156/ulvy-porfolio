<template>
  <section id="projects">
    <div class="w-fit  m-auto flex justify-center gap-x-2 items-center mt-10 mb-5 border-b-3 border-white ">
        <svg xmlns="http://www.w3.org/2000/svg" class="size-9 text-white" viewBox="0 0 32 32"><path fill="currentColor" d="M30 18H20v6.468a5.02 5.02 0 0 0 2.861 4.52L25 30l2.139-1.013A5.02 5.02 0 0 0 30 24.467zm-5 9.786l-1.283-.607A3.01 3.01 0 0 1 22 24.468V20h6v4.468a3.01 3.01 0 0 1-1.717 2.71zM17 18H5a2 2 0 0 0-2 2v5a2 2 0 0 0 2 2h12v-2H5v-5h12zM27 4h-5a2 2 0 0 0-2 2v9h2V6h5v9h2V6a2 2 0 0 0-2-2M15 4H5a2 2 0 0 0-2 2v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2M5 13V6h10v7z" stroke-width="1" stroke="currentColor"/></svg>
      <h1 class="text-center py-2 text-3xl text-white ">Projects Experienced</h1>
    </div>
    <!-- projects -->
     <section class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 justify-center gap-5 mt-10">
        <!-- project card -->
         <ClientOnly >
             <div v-for="project in projectContent" :key="project.title" data-aos="fade-up"
             class="grid  grid-cols-1 gap-5 border border-gray-600 p-3 text-white rounded-md">
                 <div class="bg-[#363636] h-40 w-full flex flex-col justify-center items-center text-center rounded-md gap-2 ">
                     <div v-html="project.svg">
                     </div>
                     <h3>{{project.title}}</h3>
                 </div>
                 <div class="grid grid-cols-1 gap-5">
                     <div class="flex items-center gap-x-2">
                         <svg xmlns="http://www.w3.org/2000/svg" class="size-7 " viewBox="0 0 24 24"><path fill="none" stroke="currentColor" stroke-width="2" d="M20 15c-1 1 1.25 3.75 0 5s-4-1-5 0s-1.5 3-3 3s-2-2-3-3s-3.75 1.25-5 0s1-4 0-5s-3-1.5-3-3s2-2 3-3s-1.25-3.75 0-5s4 1 5 0s1.5-3 3-3s2 2 3 3s3.75-1.25 5 0s-1 4 0 5s3 1.5 3 3s-2 2-3 3ZM7 12l3 3l7-7"/></svg>
                         <h3>{{project.title}}</h3>
                     </div>
                     <p class="font-light">{{project.description}}</p>
                     <article class="flex flex-wrap gap-3">
                         <p v-for="tag in project.tags" :key="tag"
                         class="bg-[#575656] px-3 py-2 rounded-full w-fit flex justify-center items-center">{{ tag }}</p>
                     </article>
                 </div>
                 <NuxtLink :to="`/project-details/${project.id}`">
                     <div class="flex items-center gap-x-2">
                         <p>View details</p>
                         <svg xmlns="http://www.w3.org/2000/svg" class="size-5" viewBox="0 0 24 24"><path fill="currentColor" d="M4 12h12.25L11 6.75l.66-.75l6.5 6.5l-6.5 6.5l-.66-.75L16.25 13H4z"/></svg>
                     </div>
                 </NuxtLink>
             </div>
         </ClientOnly>
     </section>
  </section>
</template>

<script lang="ts" setup>
import projectContent from '~/content/project.content';

</script>

<style scoped>
.border-style {
  position: relative;
  display: inline-block; /* or block, based on your layout */
}

.border-style::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  height: 4px;
  width: 100%;
  background: linear-gradient(to right, white 0%, black 100%);
  border-radius: 10px;
}

</style>
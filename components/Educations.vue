<template>
  <section id="education" class="my-10 flex flex-col gap-5">
    <div class="w-fit  m-auto flex justify-center gap-x-2 items-center mt-10 mb-5 border-b-3 border-white ">
      <svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 24 24"><path fill="currentColor" d="M6.839 15.89q-.385-.217-.612-.59Q6 14.926 6 14.462v-3.877l-1.592-.883q-.218-.13-.324-.308T3.98 9t.106-.394t.323-.308l6.82-3.72q.182-.101.375-.144T12 4.39t.397.044t.376.143l7.721 4.187q.212.125.32.313q.109.189.109.408v5.4q0 .212-.144.356t-.356.144t-.357-.144t-.143-.356V9.562L18 10.585v3.877q0 .464-.227.838t-.611.59l-4.385 2.374q-.186.105-.38.149t-.397.043t-.397-.043t-.38-.15zm4.93-3.305q.135.076.24.076q.106 0 .241-.076L18.83 9l-6.58-3.565q-.134-.077-.24-.077t-.24.077L5.17 9zm-.019 4.832q.135.077.25.077t.25-.077l4.462-2.411q.154-.096.22-.221t.068-.318v-3.332l-4.217 2.302q-.187.105-.38.149q-.191.043-.403.043t-.404-.043t-.379-.15L7 11.136v3.332q0 .154.067.299q.067.144.221.24zM12 14.36"/></svg>
      <h1 class="text-center text-3xl text-white  py-2">Educations</h1>
    </div>
    <section class="text-white grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 gap-10 ">
      <ClientOnly >
        <article v-for="edu in educationsContent" :key="edu.schoolName" class="flex flex-col gap-5 border border-gray-600 p-3 rounded-md" data-aos="fade-up">
            <NuxtImg class="m-auto" :src="edu.img" width="500" height="300" />
            <div class="flex items-center gap-x-3">
              <span v-html="edu.svg"></span>
              <h1 class="text-2xl">{{edu.schoolType}}</h1>
            </div>
            <h2 class="text-xl font-light">{{edu.schoolName}}</h2>
            <p class="font-light">{{ edu.graduated }}</p>
        </article>
      </ClientOnly>
    </section>
  </section>
</template>

<script lang="ts" setup>
import educationsContent from '~/content/educations.content';

</script>


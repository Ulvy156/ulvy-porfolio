<template>
  <section id="education" class="my-10 flex flex-col gap-5">
    <div class="flex justify-center items-center mt-10 mb-5">
      <h1 class="text-center text-3xl text-white border-style py-2">Educations</h1>
    </div>
    <section class="text-white grid lg:grid-cols-3 md:grid-cols-3 grid-cols-1 gap-10 ">
        <article v-for="edu in educations" :key="edu.schoolName" class="flex flex-col gap-5 border border-gray-600 p-3 rounded-md">
            <NuxtImg class="m-auto object-center" :src="edu.img" width="500" height="300" />
            <div class="flex items-center gap-x-3">
              <span v-html="edu.svg"></span>
              <h1 class="text-2xl">{{edu.schoolType}}</h1>
            </div>
            <h2 class="text-xl font-light">{{edu.schoolName}}</h2>
            <p class="font-light">{{ edu.graduated }}</p>
        </article>
    </section>
  </section>
</template>

<script lang="ts" setup>
useHead({
  title:"Educations"
})

const educations = readonly([
  {
    schoolType: "High School",
    schoolName:"Kroch Chhmar High School",
    graduated:"Graduated in 2020",
    img:"/assets/kpc.jpg",
    svg:`<svg xmlns="http://www.w3.org/2000/svg" class="size-7 " viewBox="0 0 48 48"><defs><mask id="ipSCheckOne0"><g fill="none" stroke-linejoin="round" stroke-width="3"><path fill="#fff" stroke="#fff" d="M24 44a19.94 19.94 0 0 0 14.142-5.858A19.94 19.94 0 0 0 44 24a19.94 19.94 0 0 0-5.858-14.142A19.94 19.94 0 0 0 24 4A19.94 19.94 0 0 0 9.858 9.858A19.94 19.94 0 0 0 4 24a19.94 19.94 0 0 0 5.858 14.142A19.94 19.94 0 0 0 24 44Z"/><path stroke="#000" stroke-linecap="round" d="m16 24l6 6l12-12"/></g></mask></defs><path fill="currentColor" d="M0 0h48v48H0z" mask="url(#ipSCheckOne0)"/></svg>`
  },
  {
    schoolType: "Associate Degree",
    schoolName:"Associate Degree in Web Development, PNC (web app training organization)",
    graduated:"Graduated in 2022",
    img:`/assets/pnc.jpg`,
    svg:`<svg xmlns="http://www.w3.org/2000/svg" class="size-7 " viewBox="0 0 48 48"><defs><mask id="ipSCheckOne0"><g fill="none" stroke-linejoin="round" stroke-width="3"><path fill="#fff" stroke="#fff" d="M24 44a19.94 19.94 0 0 0 14.142-5.858A19.94 19.94 0 0 0 44 24a19.94 19.94 0 0 0-5.858-14.142A19.94 19.94 0 0 0 24 4A19.94 19.94 0 0 0 9.858 9.858A19.94 19.94 0 0 0 4 24a19.94 19.94 0 0 0 5.858 14.142A19.94 19.94 0 0 0 24 44Z"/><path stroke="#000" stroke-linecap="round" d="m16 24l6 6l12-12"/></g></mask></defs><path fill="currentColor" d="M0 0h48v48H0z" mask="url(#ipSCheckOne0)"/></svg>`
  },
  {
    schoolType: "Bachelor Degree",
    schoolName:"Bachelor's Degree in Computer Science, AEU (University)",
    graduated:"Will graduate in 2026",
    img:`/assets/aeu.jpg`,
    svg:`<svg xmlns="http://www.w3.org/2000/svg" class='size-9' viewBox="0 0 24 24"><path fill="currentColor" d="M2 12c0 5.523 4.477 10 10 10s10-4.477 10-10S17.523 2 12 2S2 6.477 2 12m18 0a8 8 0 1 1-16 0a8 8 0 0 1 16 0m-2 0a5.98 5.98 0 0 1-1.757 4.243L12 12V6a6 6 0 0 1 6 6"/></svg>`
  }
])
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
<template>
  <section>
    <div class="flex justify-center items-center mt-10 mb-5">
      <h1 class="text-center py-2 text-3xl text-white border-style ">Feature Projects</h1>
    </div>
    <!-- projects -->
     <section class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 justify-center gap-5 mt-10">
        <!-- project card -->
        <div v-for="project in projects" :key="project.title"
        class="grid  grid-cols-1 gap-5 border border-gray-600 p-3 text-white rounded-md">
            <div class="bg-[#363636] h-40 w-full flex flex-col justify-center items-center text-center rounded-md gap-2 ">
                <div v-html="project.svg">
                </div>
                <h3>{{project.title}}</h3>
            </div>
            <div class="grid grid-cols-1 gap-5">
                <div class="flex items-center gap-x-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="size-7 text-[#646363]" viewBox="0 0 48 48"><defs><mask id="ipSCheckOne0"><g fill="none" stroke-linejoin="round" stroke-width="3"><path fill="#fff" stroke="#fff" d="M24 44a19.94 19.94 0 0 0 14.142-5.858A19.94 19.94 0 0 0 44 24a19.94 19.94 0 0 0-5.858-14.142A19.94 19.94 0 0 0 24 4A19.94 19.94 0 0 0 9.858 9.858A19.94 19.94 0 0 0 4 24a19.94 19.94 0 0 0 5.858 14.142A19.94 19.94 0 0 0 24 44Z"/><path stroke="#000" stroke-linecap="round" d="m16 24l6 6l12-12"/></g></mask></defs><path fill="currentColor" d="M0 0h48v48H0z" mask="url(#ipSCheckOne0)"/></svg>
                    <h3>{{project.title}}</h3>
                </div>
                <p class="font-light">{{project.description}}</p>
                <div class="flex flex-wrap gap-3">
                    <p v-for="tag in project.tags" :key="tag"
                    class="bg-[#575656] px-3 py-2 rounded-full w-fit flex justify-center items-center">{{ tag }}</p>
                </div>
            </div>
            <div class="flex items-center gap-x-2">
                <p>View details</p>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-5" viewBox="0 0 24 24"><path fill="currentColor" d="M4 12h12.25L11 6.75l.66-.75l6.5 6.5l-6.5 6.5l-.66-.75L16.25 13H4z"/></svg>
            </div>
        </div>
     </section>
  </section>
</template>

<script lang="ts" setup>

const projects = readonly([
    {
        title: "Official Company Website",
        description: "Dyanamic website for a company with smooth UX. Hosted on GoDaddy with Linux server for reliablity.",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","Linx", "GoDaddy", "MySQL","Element Plus"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 48 48"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="M30.79 3.6A21.2 21.2 0 0 0 24 2.5c-2.74 0-5.35.51-7.75 1.45c-5.5 2.12-9.89 6.42-12.14 11.86v.01A21.4 21.4 0 0 0 2.5 24c0 10.63 7.72 19.46 17.85 21.18h.01c1.19.21 2.4.32 3.64.32c3.76 0 7.29-.96 10.36-2.66h.01c2.84-1.57 5.28-3.75 7.16-6.39c2.5-3.51 3.97-7.8 3.97-12.45c0-2.69-.5-5.27-1.41-7.64" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="m16.238 3.944l2.035 1.615l4.267.82l-.689 2.236l-2.422.838l-2.218 3.578l-3.615 2.236l-5.068.671l-.112 2.012l1.621 1.752l-.112 2.963l-4.509-3.075l-1.302-3.777" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="m8.435 24.192l3.671-3.763l1.509 2.683l5.087.354l2.385 3.615h3.037l-.838 3.782l-2.87 2.702l-.037 2.18l-3 2.274l.093 3.764l-2.515-.932l-1.268-3.596l.056-7.379l-3.82-.69l-1.49-2.925zM37.34 15.21l1.02.08l.92-.35h.01m2.24 21.51l-2.24-1.52l-1.45-2.95l-2.82-4.96l-.09-3.24l-2.18-1.39l-3.11-.17l-5.12-2.23l-.82-4.93l2.19-2.33h2.33m-7.88 32.459l4.12-2.214l3.851-.261l2.757-.708l3.299.834" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="M44.175 10.887c-.588-1.54-7.415-6.991-7.658-7.173c-1.623-1.214-2.776-1.243-4.082-.801c-5.524 1.87-6.711 6.314-6.797 6.535a2.49 2.49 0 0 0 1.4 3.225c.303.12.616.179.924.179c.067 0 .13-.024.196-.03a2.5 2.5 0 0 0 2.462 2.83a55 55 0 0 0-1.524 2.261a2.499 2.499 0 0 0 2.107 3.842a2.5 2.5 0 0 0 2.111-1.157c2.053-3.223 4.683-6.37 6.27-7.612c.104.572.053 1.485-.577 2.433a2.5 2.5 0 1 0 4.164 2.768c1.483-2.233 1.868-5.03 1.004-7.3" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="M30.62 15.652c1.908-2.658 4.274-4.596 4.274-4.596m-6.736 1.766c1.053-1.654 3.364-3.257 3.364-3.257" stroke-width="1"/></svg>`,
        link: "https://example.com",
    },
    {
        title: "Kiva Intergration System",
        description: "Integrated Kiva’s microloan platform with company internal system",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","MS Sql Server", "API Intergration"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 640 512"><path fill="currentColor" d="M434.7 64h-85.9c-8 0-15.7 3-21.6 8.4l-98.3 90c-.1.1-.2.3-.3.4c-16.6 15.6-16.3 40.5-2.1 56c12.7 13.9 39.4 17.6 56.1 2.7c.1-.1.3-.1.4-.2l79.9-73.2c6.5-5.9 16.7-5.5 22.6 1c6 6.5 5.5 16.6-1 22.6l-26.1 23.9L504 313.8c2.9 2.4 5.5 5 7.9 7.7V128l-54.6-54.6c-5.9-6-14.1-9.4-22.6-9.4M544 128.2v223.9c0 17.7 14.3 32 32 32h64V128.2zm48 223.9c-8.8 0-16-7.2-16-16s7.2-16 16-16s16 7.2 16 16s-7.2 16-16 16M0 384h64c17.7 0 32-14.3 32-32V128.2H0zm48-63.9c8.8 0 16 7.2 16 16s-7.2 16-16 16s-16-7.2-16-16c0-8.9 7.2-16 16-16m435.9 18.6L334.6 217.5l-30 27.5c-29.7 27.1-75.2 24.5-101.7-4.4c-26.9-29.4-24.8-74.9 4.4-101.7L289.1 64h-83.8c-8.5 0-16.6 3.4-22.6 9.4L128 128v223.9h18.3l90.5 81.9c27.4 22.3 67.7 18.1 90-9.3l.2-.2l17.9 15.5c15.9 13 39.4 10.5 52.3-5.4l31.4-38.6l5.4 4.4c13.7 11.1 33.9 9.1 45-4.7l9.5-11.7c11.2-13.8 9.1-33.9-4.6-45.1" stroke-width="13" stroke="currentColor"/></svg>`,
        link: "https://example.com",
    },
    {
        title: "Disbursement System.",
        description: "Built a custom Disbursement System to manage loan releases.",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","Element Plus","MS Sql Server"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 512 512"><path fill="currentColor" d="m356.687 228.687l22.626 22.626L494.627 136L379.313 20.687l-22.626 22.626L433.372 120H16v32h417.372zM496 360H78.628l76.685-76.687l-22.626-22.626L17.373 376l115.314 115.313l22.626-22.626L78.628 392H496z" stroke-width="13" stroke="currentColor"/></svg>`,
        link: "https://example.com",
    },
]);
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
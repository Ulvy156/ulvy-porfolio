<template>
  <section class="min-h-screen text-white flex flex-col items-center">
    <!-- <div class="grid grid-cols-1 gap-5 w-1/2  " v-for="pro in matchedProjectID" :key="pro.id">
      <div class="flex items-center justify-center gap-x-2 mt-5 w-fit">
        <span v-html="pro.svg"></span>
        <h1 class="text-3xl">{{pro.title}}</h1>
      </div>
      <div class="flex items-start justify-start">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M12.02 20q-1.666 0-3.12-.626T6.36 17.66t-1.714-2.54Q4.02 13.665 4.02 12q0-1.664.626-3.12T6.36 6.34T8.9 4.626T12.02 4q1.722 0 3.281.712q1.559.711 2.718 1.984V4.808q0-.213.144-.357t.357-.143t.356.143t.143.357v2.846q0 .343-.232.575t-.575.233h-2.846q-.213 0-.357-.145q-.143-.143-.143-.356t.143-.356t.357-.144h1.98q-1.044-1.15-2.41-1.805Q13.572 5 12.02 5Q9.094 5 7.057 7.038T5.019 12t2.038 4.963T12.019 19q2.472 0 4.375-1.55t2.447-3.934q.067-.228.228-.35q.162-.124.375-.093q.227.03.333.218t.044.409q-.571 2.764-2.746 4.532T12.019 20m.5-8.208l3 3q.14.14.15.344q.01.205-.15.364q-.16.16-.354.16t-.353-.16l-3.05-3.05q-.131-.13-.187-.274t-.056-.297V7.5q0-.213.144-.356Q11.807 7 12.02 7t.356.144t.143.356z"/></svg>
        <p>Timeline: 3 months</p>
      </div>
    </div> -->
    <h1 class="text-3xl mt-5">Comming soon...</h1>
  </section>
</template>

<script lang="ts" setup>
useHead({
  title: "Project Details",
  meta: [
    {
      name: "description",
      content: "Project details page for showcasing projects.",
    },
  ],
})

const projectID = useRoute().params.id;
const projects = readonly([
    {
        id:'432fsd423',
        title: "Official Company Website",
        description: "Dyanamic website for a company with smooth UX. Hosted on GoDaddy with Linux server for reliablity.",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","Linx", "GoDaddy", "MySQL","Element Plus"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 48 48"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="M30.79 3.6A21.2 21.2 0 0 0 24 2.5c-2.74 0-5.35.51-7.75 1.45c-5.5 2.12-9.89 6.42-12.14 11.86v.01A21.4 21.4 0 0 0 2.5 24c0 10.63 7.72 19.46 17.85 21.18h.01c1.19.21 2.4.32 3.64.32c3.76 0 7.29-.96 10.36-2.66h.01c2.84-1.57 5.28-3.75 7.16-6.39c2.5-3.51 3.97-7.8 3.97-12.45c0-2.69-.5-5.27-1.41-7.64" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="m16.238 3.944l2.035 1.615l4.267.82l-.689 2.236l-2.422.838l-2.218 3.578l-3.615 2.236l-5.068.671l-.112 2.012l1.621 1.752l-.112 2.963l-4.509-3.075l-1.302-3.777" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="m8.435 24.192l3.671-3.763l1.509 2.683l5.087.354l2.385 3.615h3.037l-.838 3.782l-2.87 2.702l-.037 2.18l-3 2.274l.093 3.764l-2.515-.932l-1.268-3.596l.056-7.379l-3.82-.69l-1.49-2.925zM37.34 15.21l1.02.08l.92-.35h.01m2.24 21.51l-2.24-1.52l-1.45-2.95l-2.82-4.96l-.09-3.24l-2.18-1.39l-3.11-.17l-5.12-2.23l-.82-4.93l2.19-2.33h2.33m-7.88 32.459l4.12-2.214l3.851-.261l2.757-.708l3.299.834" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="M44.175 10.887c-.588-1.54-7.415-6.991-7.658-7.173c-1.623-1.214-2.776-1.243-4.082-.801c-5.524 1.87-6.711 6.314-6.797 6.535a2.49 2.49 0 0 0 1.4 3.225c.303.12.616.179.924.179c.067 0 .13-.024.196-.03a2.5 2.5 0 0 0 2.462 2.83a55 55 0 0 0-1.524 2.261a2.499 2.499 0 0 0 2.107 3.842a2.5 2.5 0 0 0 2.111-1.157c2.053-3.223 4.683-6.37 6.27-7.612c.104.572.053 1.485-.577 2.433a2.5 2.5 0 1 0 4.164 2.768c1.483-2.233 1.868-5.03 1.004-7.3" stroke-width="1"/><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" d="M30.62 15.652c1.908-2.658 4.274-4.596 4.274-4.596m-6.736 1.766c1.053-1.654 3.364-3.257 3.364-3.257" stroke-width="1"/></svg>`,
        link: "https://example.com",
    },
    {
        id:'481fsd423',
        title: "Kiva Intergration System",
        description: "Integrated Kiva’s microloan platform with company internal system",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","MS Sql Server", "API Intergration"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 640 512"><path fill="currentColor" d="M434.7 64h-85.9c-8 0-15.7 3-21.6 8.4l-98.3 90c-.1.1-.2.3-.3.4c-16.6 15.6-16.3 40.5-2.1 56c12.7 13.9 39.4 17.6 56.1 2.7c.1-.1.3-.1.4-.2l79.9-73.2c6.5-5.9 16.7-5.5 22.6 1c6 6.5 5.5 16.6-1 22.6l-26.1 23.9L504 313.8c2.9 2.4 5.5 5 7.9 7.7V128l-54.6-54.6c-5.9-6-14.1-9.4-22.6-9.4M544 128.2v223.9c0 17.7 14.3 32 32 32h64V128.2zm48 223.9c-8.8 0-16-7.2-16-16s7.2-16 16-16s16 7.2 16 16s-7.2 16-16 16M0 384h64c17.7 0 32-14.3 32-32V128.2H0zm48-63.9c8.8 0 16 7.2 16 16s-7.2 16-16 16s-16-7.2-16-16c0-8.9 7.2-16 16-16m435.9 18.6L334.6 217.5l-30 27.5c-29.7 27.1-75.2 24.5-101.7-4.4c-26.9-29.4-24.8-74.9 4.4-101.7L289.1 64h-83.8c-8.5 0-16.6 3.4-22.6 9.4L128 128v223.9h18.3l90.5 81.9c27.4 22.3 67.7 18.1 90-9.3l.2-.2l17.9 15.5c15.9 13 39.4 10.5 52.3-5.4l31.4-38.6l5.4 4.4c13.7 11.1 33.9 9.1 45-4.7l9.5-11.7c11.2-13.8 9.1-33.9-4.6-45.1" stroke-width="13" stroke="currentColor"/></svg>`,
        link: "https://example.com",
    },
    {
        id:'432fsdw34',
        title: "Disbursement System.",
        description: "Built a custom Disbursement System to manage loan releases.",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","Element Plus","MS Sql Server"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class="size-10 text-white" viewBox="0 0 512 512"><path fill="currentColor" d="m356.687 228.687l22.626 22.626L494.627 136L379.313 20.687l-22.626 22.626L433.372 120H16v32h417.372zM496 360H78.628l76.685-76.687l-22.626-22.626L17.373 376l115.314 115.313l22.626-22.626L78.628 392H496z" stroke-width="13" stroke="currentColor"/></svg>`,
        link: "https://example.com",
    },
    {
        id:'432fex423',
        title: "Job Seeker Web App.",
        description: "Built a Job Seeker Web Application for candidate to find a job and recruiter to find candidate.",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","Element Plus"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class='size-9' viewBox="0 0 24 24"><g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" color="currentColor"><path d="M11.007 21H9.605c-3.585 0-5.377 0-6.491-1.135S2 16.903 2 13.25s0-5.48 1.114-6.615S6.02 5.5 9.605 5.5h3.803c3.585 0 5.378 0 6.492 1.135c.857.873 1.054 2.156 1.1 4.365"/><path d="M17.111 13.255c.185-.17.277-.255.389-.255s.204.085.389.255l.713.657c.086.079.129.119.182.138c.054.02.112.018.23.013l.962-.038c.248-.01.372-.014.457.057s.102.194.135.44l.132.986c.016.114.023.17.051.22c.028.048.073.083.163.154l.776.61c.192.152.288.227.307.335s-.046.212-.174.42l-.526.847c-.06.097-.09.146-.1.2s.002.111.026.223l.209.978c.05.24.076.36.021.456s-.172.134-.405.21l-.926.301c-.11.036-.166.054-.209.09c-.043.037-.07.089-.123.192l-.452.871c-.115.223-.173.334-.278.372s-.22-.01-.452-.106l-.888-.368c-.109-.045-.163-.068-.22-.068s-.111.023-.22.068l-.888.368c-.232.096-.347.144-.452.106s-.163-.15-.278-.372l-.452-.871c-.054-.103-.08-.155-.123-.191s-.099-.055-.209-.09l-.926-.302c-.233-.076-.35-.114-.405-.21s-.03-.215.021-.456l.21-.978c.023-.112.035-.168.025-.222a.6.6 0 0 0-.1-.2l-.525-.848c-.13-.208-.194-.312-.175-.42s.115-.183.307-.334l.776-.61c.09-.072.135-.107.163-.156s.035-.105.05-.22l.133-.985c.033-.245.05-.369.135-.44s.209-.067.457-.057l.963.038c.117.005.175.007.229-.013c.053-.02.096-.059.182-.138zM16 5.5l-.1-.31c-.495-1.54-.742-2.31-1.331-2.75C13.979 2 13.197 2 11.63 2h-.263c-1.565 0-2.348 0-2.937.44c-.59.44-.837 1.21-1.332 2.75L7 5.5"/></g></svg>`,
        link: "https://example.com",
    },
    {
        id:'432fsd4qa',
        title: "Loan Delinquency System",
        description: "A robust system built to track and manage loan delinquencies.",
        tags: ["Vue JS", "Laravel", "Tailwind CSS","Element Plus","MS Sql Server","Linux"],
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class='size-9' viewBox="0 0 32 32"><path fill="currentColor" d="m15 22l-1.41 1.41L16.17 26H4V8H2v18c0 1.103.897 2 2 2h12.17l-2.58 2.59L15 32l5-5z" stroke-width="1" stroke="currentColor"/><circle cx="11" cy="16" r="1" fill="currentColor" stroke-width="1" stroke="currentColor"/><path fill="currentColor" d="M24 20H8c-1.103 0-2-.897-2-2v-4c0-1.103.897-2 2-2h16c1.103 0 2 .897 2 2v4c0 1.103-.897 2-2 2M8 14v4h16v-4z" stroke-width="1" stroke="currentColor"/><path fill="currentColor" d="M28 4H15.83l2.58-2.59L17 0l-5 5l5 5l1.41-1.41L15.83 6H28v18h2V6c0-1.102-.897-2-2-2" stroke-width="1" stroke="currentColor"/></svg>`,
        link: "https://example.com",
    },
]);

const matchedProjectID = computed(() => {
  return projects.filter((project) => {
    return project.id === projectID;
  });
})

</script>

<style></style>
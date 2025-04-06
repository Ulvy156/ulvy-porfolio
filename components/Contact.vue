<template>
    <section class="text-white grid lg:grid-cols-2 md:grid-cols-2 grid-cols-1 gap-10">
        <div class="grid grid-cols-1 gap-5">
            <div class="flex  gap-x-5">
                <h1 class="text-3xl">Let's Build Something Cool Together!</h1>
                <svg xmlns="http://www.w3.org/2000/svg" class="size-9" viewBox="0 0 64 64">
                    <path fill="#94989b"
                        d="m20.9 50.9l30-30c3.5.8 7.3-.1 10-2.8s3.6-6.5 2.8-10L55 16.7l-6.1-1.6L47.3 9L56 .3c-3.5-.8-7.3.1-10 2.8s-3.6 6.5-2.8 10l-30 30c-3.5-.8-7.3.1-10 2.8C-1 50-1 56.8 3.1 60.9s10.9 4.1 15 0c2.7-2.7 3.6-6.5 2.8-10m-8.7 8.6l-6.1-1.6l-1.6-6.1L9 47.3l6.1 1.6l1.6 6.1z"
                        stroke-width="1.5" stroke="#94989b" />
                    <path fill="#3e4347" d="m28.8 21.9l-5.6 5.8l-5.5-5.7l5.5-5.8z" stroke-width="1.5"
                        stroke="#3e4347" />
                    <path fill="#94989b"
                        d="M16.7 5.1L6.9 15.2c-.4.4-.4 1 0 1.3l3.7 3.8l3.7 3.8c.4.4.9.4 1.3 0L25.4 14c.4-.4.4-1 0-1.3L18 5.1c-.3-.4-.9-.4-1.3 0M.3 22c-.4.4-.4 1 0 1.3L7.6 31c.4.4.9.4 1.3 0c0 0 2-2.1 2.1-2.2l-8.6-8.9C2.3 19.9.3 22 .3 22"
                        stroke-width="1.5" stroke="#94989b" />
                    <path fill="#3e4347"
                        d="m10.5 20.4l-3.7-3.8s1.2 2.1-2 2.5c-1.3.2-2.1.4-2.5.8l8.6 8.9c.4-.5.6-1.3.8-2.6c.4-3.3 2.4-2 2.4-2zM39.6 4.3C29.5-6 18.4 5.5 18.4 5.5l6.5 6.7s6.3-8.5 14.2-6.1c.9.3 1.7.7 2 .5c.4-.3-.8-1.6-1.5-2.3"
                        stroke-width="1.5" stroke="#3e4347" />
                    <path fill="#f2b200"
                        d="m26 24.8l-3.6 3.7s1.9 3 5.1 6.3c3.5 3.6 8.2 5.7 12.9 10.5c7 7.2 12.8 15 14.9 17.9c.8 1.1.9 1 1.9 0l3-3.1z"
                        stroke-width="1.5" stroke="#f2b200" />
                    <path fill="#ffce31"
                        d="m26 24.8l3.6-3.7s2.9 1.9 6.1 5.2c3.5 3.6 5.5 8.5 10.2 13.3c7 7.2 14.5 13.2 17.4 15.4c1.1.8 1 1 0 2l-3 3.1z"
                        stroke-width="1.5" stroke="#ffce31" />
                </svg>
            </div>
            <div>
                <p>
                    I'm always down to talk about new projects, collaborations, or just vibe about tech and design.
                </p>
                <p>Whatever it's full-stack systems, UI/UX, or back-end intergration - I got u.</p>
                <div class="flex gap-x-2 items-center mt-5">
                    <p>Reach out via the form or hti me up on socials</p>
                    <svg xmlns="http://www.w3.org/2000/svg" class="size-6" viewBox="0 0 48 48">
                        <defs>
                            <mask id="ipTHandDown0">
                                <g fill="none" stroke="#fff" stroke-linejoin="round" stroke-width="3">
                                    <path fill="#555555" d="M7.053 10h22V4h-22z" />
                                    <path
                                        d="M29.053 10q9.78 10.684 11.222 12.384c1.443 1.7.837 3.62-2.775 3.62s-5.695-5.285-8.447-5.285q-.024-.004-.003 20.277a3 3 0 0 1-2.998 3.005h-.003a3.004 3.004 0 0 1-3.004-3.005v-8.01q-11.96-1.812-13.004-2c-1.044-.187-2.988-1.184-2.988-4.053V10z"
                                        clip-rule="evenodd" />
                                </g>
                            </mask>
                        </defs>
                        <path fill="yellow" d="M0 0h48v48H0z" mask="url(#ipTHandDown0)" />
                    </svg>
                </div>
            </div>
            <div class="grid grid-cols-1 gap-5">
                <div v-for="social in socials" :key="social.name" class="flex items-center gap-x-2">
                    <span v-html="social.svg"></span>
                    <a target="_blank" :href="social.url" class="text-lg">{{ social.name }}</a>
                </div>
            </div>
        </div>
        <form class="flex flex-col gap-5 font-light p-5 border rounded-md border-gray-800">
            <el-input v-model="inputValue" style="width: 100%" size="large" placeholder="What's your name ?">
                <template #prefix>
                    <svg xmlns="http://www.w3.org/2000/svg" class="size-5 text-black" viewBox="0 0 24 24">
                        <path fill="currentColor"
                            d="M15.71 12.71a6 6 0 1 0-7.42 0a10 10 0 0 0-6.22 8.18a1 1 0 0 0 2 .22a8 8 0 0 1 15.9 0a1 1 0 0 0 1 .89h.11a1 1 0 0 0 .88-1.1a10 10 0 0 0-6.25-8.19M12 12a4 4 0 1 1 4-4a4 4 0 0 1-4 4"
                            stroke-width="0.5" stroke="currentColor" />
                    </svg>
                </template>
            </el-input>
            <el-input v-model="inputValue" style="width: 100%" size="large" placeholder="Email">
                <template #prefix>
                    <svg xmlns="http://www.w3.org/2000/svg" class='size-5' viewBox="0 0 256 193">
                        <path fill="#4285f4"
                            d="M58.182 192.05V93.14L27.507 65.077L0 49.504v125.091c0 9.658 7.825 17.455 17.455 17.455z"
                            stroke-width="5" stroke="#4285f4" />
                        <path fill="#34a853"
                            d="M197.818 192.05h40.727c9.659 0 17.455-7.826 17.455-17.455V49.505l-31.156 17.837l-27.026 25.798z"
                            stroke-width="5" stroke="#34a853" />
                        <path fill="#ea4335"
                            d="m58.182 93.14l-4.174-38.647l4.174-36.989L128 69.868l69.818-52.364l4.669 34.992l-4.669 40.644L128 145.504z"
                            stroke-width="5" stroke="#ea4335" />
                        <path fill="#fbbc04"
                            d="M197.818 17.504V93.14L256 49.504V26.231c0-21.585-24.64-33.89-41.89-20.945z"
                            stroke-width="5" stroke="#fbbc04" />
                        <path fill="#c5221f"
                            d="m0 49.504l26.759 20.07L58.182 93.14V17.504L41.89 5.286C24.61-7.66 0 4.646 0 26.23z"
                            stroke-width="5" stroke="#c5221f" />
                    </svg>
                </template>
            </el-input>
            <el-input v-model="message" type="textarea" style="width: 100%;" size="large" placeholder="Tell me what you have in mind!">
                <template #prefix>
                    <svg xmlns="http://www.w3.org/2000/svg" class='size-5' viewBox="0 0 256 193">
                        <path fill="#4285f4"
                            d="M58.182 192.05V93.14L27.507 65.077L0 49.504v125.091c0 9.658 7.825 17.455 17.455 17.455z"
                            stroke-width="5" stroke="#4285f4" />
                        <path fill="#34a853"
                            d="M197.818 192.05h40.727c9.659 0 17.455-7.826 17.455-17.455V49.505l-31.156 17.837l-27.026 25.798z"
                            stroke-width="5" stroke="#34a853" />
                        <path fill="#ea4335"
                            d="m58.182 93.14l-4.174-38.647l4.174-36.989L128 69.868l69.818-52.364l4.669 34.992l-4.669 40.644L128 145.504z"
                            stroke-width="5" stroke="#ea4335" />
                        <path fill="#fbbc04"
                            d="M197.818 17.504V93.14L256 49.504V26.231c0-21.585-24.64-33.89-41.89-20.945z"
                            stroke-width="5" stroke="#fbbc04" />
                        <path fill="#c5221f"
                            d="m0 49.504l26.759 20.07L58.182 93.14V17.504L41.89 5.286C24.61-7.66 0 4.646 0 26.23z"
                            stroke-width="5" stroke="#c5221f" />
                    </svg>
                </template>
            </el-input>
            <div class="text-white rounded-md p-2 border flex justify-center items-center gap-x-3">
                <button>Send Message</button>
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="m14 10l-3 3m9.288-9.969a.535.535 0 0 1 .68.681l-5.924 16.93a.535.535 0 0 1-.994.04l-3.219-7.242a.54.54 0 0 0-.271-.271l-7.242-3.22a.535.535 0 0 1 .04-.993z"/></svg>
            </div>
        </form>
    </section>

</template>

<script lang="ts" setup>

const inputValue = ref<string>('')
const message = ref<string>("")
const socials = readonly([
    {
        url:'https://github.com/Ulvy156',
        name: 'GitHub',
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class='size-7 ' viewBox="0 0 2048 2048"><path fill="currentColor" d="M1024 25q141 0 272 36t244 104t207 160t161 207t103 245t37 272q0 165-50 318t-143 281t-221 224t-286 149q-3 1-9 1t-9 1q-24 0-38-14t-14-37v-140q0-69 1-141q0-51-15-103t-54-87q116-13 203-47t146-96t88-150t30-212q0-78-26-147t-79-128q11-28 16-58t5-60q0-39-8-77t-23-76q-5-2-11-2t-11 0q-32 0-67 10t-69 26t-67 35t-57 36q-125-35-256-35t-256 35q-25-17-57-36t-66-34t-70-26t-67-11h-11q-6 0-11 2q-14 37-22 75t-9 78q0 30 5 60t16 58q-53 58-79 127t-26 148q0 122 29 211t88 150t146 97t203 48q-29 26-44 62t-21 75q-27 13-57 20t-60 7q-64 0-106-30t-75-82q-12-19-29-38t-37-34t-43-24t-48-10h-12q-8 0-15 3t-14 6t-6 10q0 12 14 23t23 18l3 2q22 17 38 32t30 33t23 38t23 47q34 78 95 113t147 36q26 0 52-3t52-9v174q0 24-14 38t-39 14h-8q-5 0-9-2q-157-51-286-147t-221-225t-142-282t-51-318q0-141 36-272t104-244t160-207t207-161T752 62t272-37"/></svg>`
    },
    {
        url:'www.linkedin.com/in/ulvy-romy',
        name: 'LinkedIn',
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class='size-8' viewBox="0 0 24 24"><g fill="none" stroke="#0076b2" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" color="#0076b2"><path d="M7 10v7m4-4v4m0-4a3 3 0 1 1 6 0v4m-6-4v-3M7.008 7h-.009"/><path d="M2.5 12c0-4.478 0-6.718 1.391-8.109S7.521 2.5 12 2.5c4.478 0 6.718 0 8.109 1.391S21.5 7.521 21.5 12c0 4.478 0 6.718-1.391 8.109S16.479 21.5 12 21.5c-4.478 0-6.718 0-8.109-1.391S2.5 16.479 2.5 12"/></g></svg>`
    },
    {
        url:'mailto:ulvyromy156@gmail.com',
        name: 'ulvyromy156@gmail.com',
        svg: `<svg xmlns="http://www.w3.org/2000/svg" class='size-8' viewBox="0 0 256 193"><path fill="#4285f4" d="M58.182 192.05V93.14L27.507 65.077L0 49.504v125.091c0 9.658 7.825 17.455 17.455 17.455z" stroke-width="5" stroke="#4285f4"/><path fill="#34a853" d="M197.818 192.05h40.727c9.659 0 17.455-7.826 17.455-17.455V49.505l-31.156 17.837l-27.026 25.798z" stroke-width="5" stroke="#34a853"/><path fill="#ea4335" d="m58.182 93.14l-4.174-38.647l4.174-36.989L128 69.868l69.818-52.364l4.669 34.992l-4.669 40.644L128 145.504z" stroke-width="5" stroke="#ea4335"/><path fill="#fbbc04" d="M197.818 17.504V93.14L256 49.504V26.231c0-21.585-24.64-33.89-41.89-20.945z" stroke-width="5" stroke="#fbbc04"/><path fill="#c5221f" d="m0 49.504l26.759 20.07L58.182 93.14V17.504L41.89 5.286C24.61-7.66 0 4.646 0 26.23z" stroke-width="5" stroke="#c5221f"/></svg>`
    }
])
</script>

<style scoped>
p {
    font-weight: lighter;
}
</style>
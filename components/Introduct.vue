<template>
    <ClientOnly >
        <section data-aos="fade-up" class="text-white grid grid-cols-1 gap-5">
              <h1 class="text-3xl">Hi, I'm Ulvy</h1>
              <div class="flex text-gray-300 items-center gap-x-2">
                  <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M3 7V4h18v3h-1V5H4v2zm6 13v-2H3v-3h1v2h16v-2h1v3h-6v2zm-4.584-9l2.6-2.6l-.708-.708L3 11l3.308 3.308l.708-.708zm15.169 0l-2.6 2.6l.707.708L21 11l-3.308-3.308l-.707.708z"/></svg>
                  <h3 class="text-xl ">
                      Full-stack developer
                  </h3>
              </div>
              <p class="font-light">I specialize in buidling internal systems that actually work fast, secure, and clean, I handle everything from front-end interfaces  in Vue 3+ + Tailwind to backend logic with Laravel
                  and Nest JS.
              </p>
              <p class="font-light">
                  I have built systems for up to 200+ users that run smoothly over local networks & VPN. Design matters to me, I always try to make the user experience as seamless as possible. I am also a big fan of open source software and I love to contribute to it.
              </p>
              <p class="font-light">
                  I work solo, move fast, and ship with purpose. Let's build something great together!
              </p>
        </section>
    </ClientOnly>
</template>

<script lang="ts" setup>
useHead({
  title:"Introduction",
})
</script>

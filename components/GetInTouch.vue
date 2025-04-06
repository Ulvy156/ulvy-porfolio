<template>
  <section id="git-in-touch" class="text-white flex justify-between items-center ">
    <div class="grid grid-cols-1 gap-5">

      <div>
        <h1 class="text-5xl">Full-Stack Developer</h1>
        <p class="font-light">Designing seamless experiences, building powerful apps</p>
      </div>
      <div class="grid lg:grid-cols-2 md:grid-cols-2 grid-cols-1 gap-5">
        <div class="border border-gray-300 rounded-full w-fit p-2 flex gap-x-2 items-center">
          <div class="custom-loader"></div>
          <!-- <svg xmlns="http://www.w3.org/2000/svg" class="size-9" viewBox="0 0 24 24"><path fill="currentColor" d="M12 10a2 2 0 0 0-2 2a2 2 0 0 0 2 2c1.11 0 2-.89 2-2a2 2 0 0 0-2-2"/></svg> -->
          <h3>Available for projects</h3>
        </div>
        <div class="bg-white w-fit text-black p-2 rounded-full flex items-center  gap-x-1">
          <button >Get In Touch</button>
          <svg xmlns="http://www.w3.org/2000/svg" class="size-7" viewBox="0 0 24 24"><path fill="currentColor" d="M4 12h12.25L11 6.75l.66-.75l6.5 6.5l-6.5 6.5l-.66-.75L16.25 13H4z" stroke-width="0.5" stroke="currentColor"/></svg>
        </div>
      </div>
    </div>
    <div class=" lg:flex md:flex justify-center w-1/3  border-2 rounded-full">
      <img src="~/public/assets/profile.jpg" class="relative object-cover rounded-full" alt="profile picture">
      <!-- <img src="~/public/assets/programming.svg"  alt="profile picture"> -->
       <!-- <div v-html="profile"></div> -->
    </div>
  </section>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.custom-loader {
  width: 25px;
  height: 25px;
  display: grid;
  color:white;
  background: radial-gradient(farthest-side, currentColor calc(100% - 3px),#0000 calc(100% - 2.5px) 0);
  -webkit-mask:radial-gradient(farthest-side,#0000 calc(100% - 6.5px),#000 calc(100% - 6px));
  border-radius: 50%;
  animation: s9 2s infinite linear;
}
.custom-loader::before,
.custom-loader::after {    
  content:"";
  grid-area: 1/1;
  background:
    linear-gradient(currentColor 0 0) center,
    linear-gradient(currentColor 0 0) center;
  background-size: 100% 5px,5px 100%;
  background-repeat: no-repeat;
}
.custom-loader::after {
   transform: rotate(45deg);
}

@keyframes s9 { 
  100%{transform: rotate(1turn)}
}


</style>
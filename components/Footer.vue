<template>
    <footer class="w-11/12 m-auto border-t border-gray-500 p-3 text-center mb-5">
        <p class="text-white">@ {{ year }} Ulvy. All Right Reserved.</p>
    </footer>
</template>

<script setup lang="ts">

const year = new Date().getFullYear();

</script>
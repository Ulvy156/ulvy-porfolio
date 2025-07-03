<template>
  <section class="my-10 grid grid-cols-1 gap-10">
    <GetInTouch/>
    <Introduct/>
    <Educations/>
    <SkillsTools/>
    <FeatureProjects/>
    <Contact/>
  </section>
</template>

<script lang="ts" setup>
definePageMeta({
  title: 'Ulvy Portfolio',
  meta: [
    { name: 'description', content: 'I specialize in buidling internal systems that actually work fast, secure, and clean, I handle everything from front-end interfaces in Vue 3+ + Tailwind to backend logic with Laravel and Nest JS.' },
  ]
})
import GetInTouch from '~/components/GetInTouch.vue';
import Introduct from '~/components/Introduct.vue';
import SkillsTools from '~/components/SkillsTools.vue';
import FeatureProjects from '~/components/FeatureProjects.vue';
import Contact from '~/components/Contact.vue';
import Educations from '~/components/Educations.vue';
</script>


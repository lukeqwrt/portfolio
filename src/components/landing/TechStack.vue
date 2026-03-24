<script setup>
import { ref } from 'vue'
import html from '../../assets/skills/html.png'
import css from '../../assets/skills/css.png'
import js from '../../assets/skills/js.png'
import tailwind from '../../assets/skills/tailwind.png'
import bootstrap from '../../assets/skills/bootstrap.png'
import sass from '../../assets/skills/sass.png'
import firebase from '../../assets/skills/firebase.png'
import vue from '../../assets/skills/vuejs.png'
import wordpress from '../../assets/skills/wordpress.png'
import elementor from '../../assets/skills/elementor.png'
import react from '../../assets/skills/react.png'
import git from '../../assets/skills/git.png'
import figma from '../../assets/skills/figma.png'


const techStack = ref([html, css, js, tailwind, bootstrap, sass, firebase , vue, git, react, wordpress, elementor, figma])

</script>

<template>
    <div class="tech pe-2 flex items-start gap-4 absolute bottom-0 left-0 sm:left-0  md:left-0 md:bottom-0 md:gap-5">
        <div class="flex gap-3 md:gap-5 justify-between items-center">
            <span class="font-bold text-sm md:whitespace-nowrap lg:text-lg ">Tech Stack </span>
            <div class="font-[400] block">|</div> 
        </div>
        <!-- <div class="w-[1px] self-stretch bg-[#000]"></div> -->
        <ul class="tech-logo flex items-center flex-wrap gap-5 md:gap-7 lg:gap-8">
            <li v-for="skill in techStack" :key="skill">
                <img :src="skill" class="h-[auto] w-[20px] md:h-[auto] md:w-[25px] lg:h-[auto] lg:w-[30px]">
            </li>
        </ul>
    </div>
</template>
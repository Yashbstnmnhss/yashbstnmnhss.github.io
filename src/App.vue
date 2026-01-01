<script setup lang="ts">
import { NText, NH1, NDivider, NInfiniteScroll, NBlockquote, NCard } from 'naive-ui'
import LOGO from './assets/main_logo.svg'
</script>

<template>
    <div class="slide center">
        <img :src="LOGO" style="width: 60vw" />
        <NH1><NText code style="font-size: 1.75vw">Website of Unknown</NText> </NH1>
    </div>
    <NDivider />
    <div class="slide"></div>
</template>

<style>
#app {
    scroll-snap-type: mandatory;
}
body {
    margin: 0;
    min-height: 100vh;
    padding-left: 0.5rem;
    padding-right: 0.5rem;
}
.center {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    user-select: none;
}
.slide {
    scroll-snap-align: center;
    min-height: 100vh;
}
</style>

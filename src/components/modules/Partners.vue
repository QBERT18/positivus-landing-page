<script setup lang="ts">
const images = [
    "/src/assets/amazon.svg",
    "/src/assets/dribble.svg",
    "/src/assets/hubspot.svg",
    "/src/assets/notion.svg",
    "/src/assets/netflix.svg",
    "/src/assets/zoom.svg",
];
</script>

<template>
    <div
        class="grid grid-cols-[repeat(auto-fit,_minmax(150px,_1fr))] place-items-center lg:px-[100px] mt-[80px] lg:mt-[100px]">
        <img v-for=" (img, index) in images" :key="index" :src="img" alt="Image" class="w-[125px] h-auto rounded-lg" />
    </div>
</template>


<style scoped></style>
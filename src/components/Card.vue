<script setup lang="ts">
import Link from './Link.vue';

defineProps<{ headline: string; link: string; linkText: string; image: string, extraClasses?: string }>();
</script>

<template>
    <div class="rounded-[45px] border [box-shadow:0px_5px_0px_#191a23] bg-aqua-haze border-mirage">
        <div>
            <div>{{ headline }}</div>
            <div>
                <img :src=image alt="search engine optimization">
            </div>
        </div>
        <Link type="white-lime" linkText="Learn more (white-lime)" />
        <Link type="white-black" linkText="Learn more (white-black)" />
        <Link type="black-lime" linkText="Learn more (black-lime)" />
        <Link type="black-white" linkText="Learn more (black-white)" />
        <Link type="lime-black" linkText="Learn more (lime-black)" />
        <Link type="lime-white" linkText="Learn more (lime-white)" />
    </div>
</template>

<style scoped></style>

<script setup lang="ts">
import Headline from '../Headline.vue';
import Paragraph from '../Paragraph.vue';
import Button from '../Button.vue';

</script>

<template>
    <div class="grid lg:grid-cols-[1fr_1fr] lg:grid-rows-[1fr_1fr] px-[20px] lg:px-[100px]">
        <Headline extraClasses="self-end" type="h1" text="Navigating the digital landscape for success" />
        <div class="px-[34px] mt-[10px] lg:mt-0 lg:row-span-2 self-center">
            <img src="/src/assets/Illustration-desktop.svg" alt="Illustration" width="100%">
        </div>
        <div class="mt-[20px] lg:mt-[35px]">
            <Paragraph
                text="Our digital marketing agency helps businesses grow and succeed online through a range of services including SEO, PPC, social media marketing, and content creation." />
            <Button extraClasses="mt-[40px] lg:mt-[35px] lg:w-[264px]" type="primary" text="Book a consultation" />
        </div>
    </div>
</template>

<style scoped></style>
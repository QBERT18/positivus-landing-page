<script setup lang="ts">
defineProps<{ type: string; text: string; extraClasses?: string }>();
</script>

<template>
    <component :is="type" :class="[
        'font-medium font-[\'Space_Grotesk\',_serif] text-left',
        {
            'tracking-[0px] text-[43px] sm:text-[60px]': type === 'h1',
            'tracking-[0px] text-[36px] sm:text-[40px]': type === 'h2',
            'tracking-[0px] text-[26px] sm:text-[30px]': type === 'h3',
            'tracking-[0px] text-[18px] sm:text-[20px]': type === 'h4',
        },
        extraClasses
    ]">
        {{ text }}
    </component>
</template>

<style scoped></style>

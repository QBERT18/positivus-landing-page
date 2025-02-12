<script setup lang="ts">
defineProps<{ text: string; extraClasses?: string }>();
</script>

<template>
    <p :class="[
        'font-normal text-[16px] sm:text-[18px] font-[\'Space_Grotesk\',_serif]',
        extraClasses
    ]">
        {{ text }}
    </p>
</template>

<style scoped></style>

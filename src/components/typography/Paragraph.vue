<script setup lang="ts">
defineProps<{ text: string }>()
</script>

<template>
    <p class="text-black font-normal text-[18px] font-['Space_Grotesk',_serif]">{{ text }}</p>
</template>

<style scoped></style>
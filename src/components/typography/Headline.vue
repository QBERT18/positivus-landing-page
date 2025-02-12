<script setup lang="ts">
defineProps<{ type: string; text: string }>()
</script>

<template>
    <h1 class="text-black font-medium text-[60px] font-['Space_Grotesk',_serif]" v-if="type === 'h1'">{{ text }}</h1>
    <h2 class="text-black font-medium text-[40px] font-['Space_Grotesk',_serif]" v-if="type === 'h2'">{{ text }}</h2>
    <h3 class="text-black font-medium text-[30px] font-['Space_Grotesk',_serif]" v-if="type === 'h3'">{{ text }}</h3>
    <h4 class="text-black font-medium text-[20px] font-['Space_Grotesk',_serif]" v-if="type === 'h4'">{{ text }}</h4>
</template>

<style scoped></style>
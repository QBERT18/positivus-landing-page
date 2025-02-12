<script setup lang="ts">
defineProps<{ type: 'primary' | 'secondary' | 'tertiary'; text: string; extraClasses?: string }>();
</script>

<template>
    <button :class="[
        'rounded-[14px] px-[35px] py-[20px] w-full font-medium',
        {
            'bg-mirage text-white': type === 'primary',
            'border border-mirage': type === 'secondary',
            'bg-pale-lime text-black': type === 'tertiary',
        },
        extraClasses
    ]">
        {{ text }}
    </button>
</template>

<style scoped></style>

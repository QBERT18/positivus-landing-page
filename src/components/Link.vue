<script setup lang="ts">
import { computed } from "vue";

const props = defineProps<{
    type?: 'white-lime' | 'white-black' | 'black-lime' | 'black-white' | 'lime-black' | 'lime-white' | 'simple-black' | 'simple-white' | 'simple-lime';
    target?: '_self' | '_blank' | '_parent' | '_top';
    linkPath?: string;
    linkText?: string;
    extraClasses?: string;
}>();

const circleFill = computed(() => {
    switch (props.type) {
        case 'white-lime': return '#FFFFFF';
        case 'white-black': return '#FFFFFF';
        case 'black-lime': return '#191A23';
        case 'black-white': return '#191A23';
        case 'lime-black': return '#B9FF66';
        case 'lime-white': return '#B9FF66';
        case 'simple-black': return '#191A23';
        case 'simple-white': return '#FFFFFF';
        case 'simple-lime': return '#B9FF66';
        default: return '#191A23';
    }
});

const arrowFill = computed(() => {
    switch (props.type) {
        case 'white-lime': return '#B9FF66';
        case 'white-black': return '#000000';
        case 'black-lime': return '#B9FF66';
        case 'black-white': return '#FFFFFF';
        case 'lime-black': return '#000000';
        case 'lime-white': return '#FFFFFF';
        case 'simple-black': return '#000000';
        case 'simple-white': return '#000000';
        case 'simple-lime': return '#000000';
        default: return '#B9FF66';
    }
});
</script>

<template>
    <span class="flex items-center gap-x-[6.5px]">
        <svg width="41" height="41" viewBox="0 0 41 41" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="20.5" cy="20.5" r="20.5" :fill="circleFill" />
            <path
                d="M11.2501 24.7009C10.5326 25.1151 10.2868 26.0325 10.701 26.75C11.1152 27.4674 12.0326 27.7132 12.7501 27.299L11.2501 24.7009ZM30.7694 16.3882C30.9839 15.588 30.509 14.7655 29.7088 14.5511L16.6688 11.057C15.8686 10.8426 15.0461 11.3175 14.8317 12.1177C14.6173 12.9179 15.0921 13.7404 15.8923 13.9548L27.4834 17.0606L24.3776 28.6517C24.1632 29.4519 24.6381 30.2744 25.4383 30.4888C26.2385 30.7033 27.061 30.2284 27.2754 29.4282L30.7694 16.3882ZM12.7501 27.299L30.0706 17.299L28.5706 14.7009L11.2501 24.7009L12.7501 27.299Z"
                :fill="arrowFill" />
        </svg>

        <a :href="linkPath || '#'" :target="target || '_self'"
            :class="['text-[20px] font-normal tracking-[0px] text-left', extraClasses]">
            {{ linkText || 'Default Link' }}
        </a>
    </span>
</template>

<style scoped></style>

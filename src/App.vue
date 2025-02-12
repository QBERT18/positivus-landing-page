<script setup lang="ts">
import Headline from './components/typography/Headline.vue'
import Paragraph from './components/typography/Paragraph.vue';
</script>

<template>
  <div>
    <Headline type="h1" text="Headline 1" />
    <Headline type="h2" text="Headline 2" />
    <Headline type="h3" text="Headline 3" />
    <Headline type="h4" text="Headline 4" />
    <Paragraph text="Paragraph" />
  </div>
</template>

<style scoped></style>
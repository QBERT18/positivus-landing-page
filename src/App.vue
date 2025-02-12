<script setup lang="ts">
import Partners from './components/modules/Partners.vue';
import Services from './components/modules/Services.vue';
import Stage from './components/modules/Stage.vue';
</script>

<template>
  <div class="w-full">
    <Services />
    <Stage />
    <Partners />
  </div>
</template>

<style scoped>
html,
body {
  width: 100%;
  overflow-x: hidden;
}
</style>
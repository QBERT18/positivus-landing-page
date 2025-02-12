<script setup lang="ts">
import Card from '../Card.vue';
import Headline from '../Headline.vue';
import Paragraph from '../Paragraph.vue';

</script>

<template>
    <div class="">
        <div>
            <Headline type="h2" text="Services" />
            <Paragraph
                text="At our digital marketing agency, we offer a range of services to help businesses grow and succeed online. These services include:" />
        </div>
        <div>
            <Card headline="Search engine optimization" image="/src/assets/search-engine.svg" link="https://www.google.com" link-text="Learn more" />
        </div>
    </div>
</template>

<style scoped></style>
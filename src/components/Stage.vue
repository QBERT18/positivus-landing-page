<script setup lang="ts">
</script>

<template>

    <section class="grid xl:grid-cols-2 px-[20px] xl:px-[100px]">
        <h1 class="stage-headline xl:self-end">
            Navigating the digital landscape for success
        </h1>
        <img class="w-full xl:row-span-2 mt-[10px] xl:mt-0" src="../assets/stage-illustration.svg"
            alt="Illustration of digital marketing services" loading="lazy">
        <div class="mt-[20px] xl:mt-[35px]">
            <p class="stage-text">
                Our digital marketing agency helps businesses grow and succeed online through a range of services
                including
                SEO, PPC, social media marketing, and content creation.
            </p>
            <button class="stage-button mt-[40px] xl:mt-[35px] py-[20px] px-[35px]">
                Book a consultation
            </button>
        </div>
    </section>

</template>

<style scoped>
.stage-headline {
    font-weight: 500;
    font-size: 43px;
    line-height: 55px;
    color: #000000;
}

.stage-text {
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    color: #000000;
}

.stage-button {
    width: 100%;
    background: #191A23;
    border-radius: 14px;
    font-weight: 400;
    font-size: 20px;
    line-height: 28px;
    text-align: center;
    color: #FFFFFF;
    cursor: pointer;
}

.stage-button:focus {
    outline: 2px solid #191A23;
    outline-offset: 2px;
}

@media (width >=80rem) {
    .stage-headline {
        font-weight: 500;
        font-size: 60px;
        line-height: 77px;
        color: #000000;
    }

    .stage-text {
        font-weight: 400;
        font-size: 20px;
        line-height: 28px;
        color: #000000;
    }

    .stage-button {
        width: 264px;
    }
}
</style>
<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    methods: {
        scrollbottom() {
            window.scrollTo(0, document.body.scrollHeight);
        }
    }
});
</script>

<template>
    <div class="md:mt-[45px] md:flex md:justify-between md:items-top overflow-hidden mt-[48px] md:px-[56px] px-[16px]">
        <div class="w-fit h-fit">
            <img src="/img/dolaposee.png" class="w-full md:w-[98%]" alt="" />
        </div>
        <div @click="scrollbottom" class="hidden cursor-pointer md:flex">
            <img src="/img/scrollicon.svg" class="" alt="" />
        </div>
    </div>
</template>

<style scoped>

</style>
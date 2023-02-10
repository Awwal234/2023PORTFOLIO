<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    components: {
    },
    mounted() {
        this.printdate()
    },
    data() {
        return {
            timed: ''
        }
    },
    methods: {
        printdate() {
            const date = new Date();
            const hours = date.getHours();
            const minutes = date.getMinutes();
            const ampm = hours >= 12 ? 'PM' : 'AM';
            const hours12 = hours % 12 || 12;

            const time = `${hours12}  : ${minutes < 10 ? '0' : ''}${minutes} ${ampm}`;

            this.timed = time
        },
    },
});
</script>

<template>
    <header class="md:pt-[30px] h-fit w-full flex items-center justify-between md:px-[56px] pt-[40px] px-[16px]">
        <div>
            <img src="/img/FMD.svg" class="" alt="" />
        </div>
        <div class="items-center hidden md:flex">
            <div
                class="text-[#221115] cursor-pointer text-center lg:w-[225px] w-[200px] h-fit p-[8px] text-[14px] font-[600] leading-[17.64px]">
                AboutHIM
            </div>
            <div class="h-[34px] line"></div>
            <div
                class="text-[#221115] cursor-pointer text-center lg:w-[225px] w-[200px] h-fit p-[8px] text-[14px] font-[600] leading-[17.64px]">
                art-icles
            </div>
        </div>
        <div class="md:flex space-x-[5px] items-center hidden">
            <div><img src="/img/BubleFlash.svg" class="" alt="" /></div>
            <div class="font-[600] text-[14px] leading-[17.64px] text-[#221115]">{{ timed }}</div>
        </div>
        <div class="md:hidden">
            <img src="/img/menuicon.svg" class="w-[24px] h-[24px]" alt="" />
        </div>
    </header>
</template>

<style scoped>
.line {
    border-width: 1px;
    border-image: linear-gradient(rgba(6, 40, 55, 1) rgba(6, 40, 55, 0), rgba(6, 40, 55, 0) rgba(6, 40, 55, 1));
}
</style>
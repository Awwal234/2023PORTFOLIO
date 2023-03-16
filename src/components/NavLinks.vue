<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    components: {
    },
    created(){
        this.printdate()
    },
    data() {
        return {
            timed: '',
            menu: false,
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
        articles() {
            window.location.href = "https://medium.com/@fabowalemuhawwal"
        },
        togglemenu() {
            this.menu = !this.menu
        },
    },
});
</script>

<template>
    <div>
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
                <div @click="articles"
                    class="text-[#221115] cursor-pointer text-center lg:w-[225px] w-[200px] h-fit p-[8px] text-[14px] font-[600] leading-[17.64px]">
                    art-icles
                </div>
            </div>
            <div class="md:flex space-x-[5px] items-center hidden">
                <div><img src="/img/BubleFlash.svg" class="" alt="" /></div>
                <div class="font-[600] text-[14px] leading-[17.64px] text-[#221115]">{{ timed }}</div>
            </div>
            <div @click="togglemenu" class="md:hidden">
                <img src="/img/menuicon.svg" class="w-[24px] h-[24px]" alt="" />
            </div>
        </header>

        <div v-show="menu" class="md:hidden bg-[#221115] w-full fixed top-0 py-[40px] left-0 z-[1000] h-full">
            <div class="px-[16px] flex items-center justify-between">
                <div class="w-fit h-fit"><img src="/img/menulogo.svg" class="" alt="" /></div>
                <div class="w-fit h-fit" @click="togglemenu"><img src="/img/menuno.png" class="w-[46px] h-[46px]"
                        alt="" /></div>
            </div>
            <div class="border-[1px] border-[#30181D] w-full mt-[24px]"></div>
            <div class="px-[16px] font-[700] font-['panchang'] mt-[67px] text-[#fff] text-[48px]">Menu</div>
            <div class="px-[16px] w-full">
                <div @click="togglemenu"
                    class="p-[16px] border-[1px] border-[#30181D] w-full mt-[32px] flex justify-between items-center">
                    <div class="font-[700] text-[#fff] text-[24px]">About Him</div>
                    <div><img src="/img/Starz.svg" class="" alt="" /></div>
                </div>
            </div>
            <div class="px-[16px] w-full">
                <div @click="articles"
                    class="p-[16px] border-[1px] border-[#30181D] w-full flex justify-between items-center">
                    <div class="font-[700] text-[#fff] text-[24px]">art-icles</div>
                    <div><img src="/img/Starz.svg" class="" alt="" /></div>
                </div>
            </div>
        </div>
        <!--end all the gbogbo-->
    </div>
</template>

<style scoped>
.line {
    border-width: 1px;
    border-image: linear-gradient(rgba(6, 40, 55, 1) rgba(6, 40, 55, 0), rgba(6, 40, 55, 0) rgba(6, 40, 55, 1));
}
</style>
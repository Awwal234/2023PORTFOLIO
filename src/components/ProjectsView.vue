<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    components: {
    },
    mounted() {

    },
    data() {
        return {
            mono: false,
            alts: false,
            nfts: false,
            norebase: false,
            tred: false,
            easy: false,
        }
    },
    methods: {
        showmono() {
            this.mono = !this.mono
        },
        showalts() {
            this.alts = !this.alts
        },
        shownfts() {
            this.nfts = !this.nfts
        },
        shownorebase() {
            this.norebase = !this.norebase
        },
        showeasy() {
            this.easy = !this.easy
        },
        showtred() {
            this.tred = !this.tred
        },
    },
});
</script>

<template>
    <div class="mt-[72px] md:mt-[88px] px-[16px] md:px-[56px]">
        <div class="md:flex items-stretch">
            <div class="w-full md:w-[50%] md:h-fit">
                <div class="w-fit h-fit"><img src="/img/AAkid.png" class="md:w-[674px] md:h-[653px]" alt="" /></div>
                <div class="w-full hidden md:flex relative mt-[-150px] left-[10px]  justify-end">
                    <div class="w-fit h-fit">
                        <img src="/img/Artifact.png" class="w-[389px] h-[389px]" alt="" />
                    </div>
                </div>
                <div v-show="mono" class="hidden md:flex relative top-[-270px] left-[-90px] justify-end">
                    <div class="w-fit h-fit"><img src="/img/Mono.png" class="w-[237px] h-[146px]" alt="" /></div>
                </div>
                <div v-show="alts" class="hidden md:flex relative top-[-270px] left-[-90px] justify-end">
                    <div class="w-fit h-fit"><img src="/img/Alts.png" class="w-[237px] h-[146px]" alt="" /></div>
                </div>
                <div v-show="nfts" class="hidden md:flex relative top-[-270px] left-[-90px] justify-end">
                    <div class="w-fit h-fit"><img src="/img/NFT.png" class="w-[237px] h-[146px]" alt="" /></div>
                </div>
                <div v-show="norebase" class="hidden md:flex relative top-[-270px] left-[-90px] justify-end">
                    <div class="w-fit h-fit"><img src="/img/Norebase.png" class="w-[237px] h-[146px]" alt="" /></div>
                </div>
                <div v-show="easy" class="hidden md:flex relative top-[-270px] left-[-90px] justify-end">
                    <div class="w-fit h-fit"><img src="/img/Easybuddy.png" class="w-[237px] h-[146px]" alt="" /></div>
                </div>
                <div v-show="tred" class="hidden md:flex relative top-[-270px] left-[-90px] justify-end">
                    <div class="w-fit h-fit"><img src="/img/TredFinance.png" class="w-[237px] h-[146px]" alt="" />
                    </div>
                </div>
            </div>
            <!----->
            <div class="md:hidden mx-auto relative mt-[-110px] w-fit h-fit">
                <img src="/img/Artifact.png" class="w-[195px] h-[195px]" alt="" />
            </div>
            <div v-show="mono" class="md:hidden relative top-[-140px] left-[-17px] mx-auto justify-end">
                <div class="w-fit mx-auto h-fit"><img src="/img/Mono.png" class="w-[118.8px] mx-auto h-[73.19px]"
                        alt="" />
                </div>
            </div>
            <div v-show="alts" class="md:hidden relative top-[-140px] left-[-17px] mx-auto justify-end">
                <div class="w-fit mx-auto h-fit"><img src="/img/Alts.png" class="w-[118.8px] mx-auto h-[73.19px]"
                        alt="" />
                </div>
            </div>
            <div v-show="nfts" class="md:hidden relative top-[-140px] left-[-17px] mx-auto justify-end">
                <div class="w-fit mx-auto h-fit"><img src="/img/NFT.png" class="w-[118.8px] mx-auto h-[73.19px]"
                        alt="" /></div>
            </div>
            <div v-show="norebase" class="md:hidden relative top-[-140px] left-[-17px] mx-auto justify-end">
                <div class="w-fit mx-auto h-fit"><img src="/img/Norebase.png" class="w-[118.8px] mx-auto h-[73.19px]"
                        alt="" />
                </div>
            </div>
            <div v-show="easy" class="md:hidden relative top-[-140px] left-[-17px] mx-auto justify-end">
                <div class="w-fit mx-auto h-fit"><img src="/img/Easybuddy.png" class="w-[118.8px] mx-auto h-[73.19px]"
                        alt="" />
                </div>
            </div>
            <div v-show="tred" class="md:hidden relative top-[-140px] left-[-17px] mx-auto justify-end">
                <div class="w-fit mx-auto h-fit"><img src="/img/TredFinance.png" class="w-[118.8px] mx-auto h-[73.19px]"
                        alt="" />
                </div>
            </div>
            <!---->
            <div
                class="w-full mt-[16px] md:mt-[0px] bg-[#ECEBE9] md:h-fit md:border-[1px] md:border-[#C2BEB8] px-[16px] py-[24px] md:w-[50%]">
                <div @mouseenter="showmono()" @mouseleave="showmono()"
                    class="font-[700] font-['panchang'] cursor-pointer text-[24px] tx_stroke text-right text-[transparent] flex justify-end md:text-[30px] lg:text-[40px] hover:text-[#221115]">
                    <div>Mono Clone</div>
                </div>
                <div class="border-[1px] border-[#C1BEB8] w-full"></div>
                <div @mouseenter="showalts()" @mouseleave="showalts()"
                    class="font-[700] cursor-pointer mt-[48px] font-['panchang'] text-[24px] tx_stroke text-[transparent] text-right flex justify-end md:text-[30px] lg:text-[40px] hover:text-[#221115]">
                    <div>Alt~School Clone</div>
                </div>
                <div class="border-[1px] border-[#C1BEB8] w-full"></div>
                <div @mouseenter="shownfts()" @mouseleave="shownfts()"
                    class="font-[700] cursor-pointer mt-[48px] font-['panchang'] text-[24px] tx_stroke text-[transparent] text-right flex justify-end md:text-[30px] lg:text-[40px] hover:text-[#221115]">
                    <div>NFTsHOT</div>
                </div>
                <div class="border-[1px] border-[#C1BEB8] w-full"></div>
                <div @mouseenter="shownorebase()" @mouseleave="shownorebase()"
                    class="font-[700] cursor-pointer mt-[48px] font-['panchang'] text-[24px] tx_stroke text-[transparent] text-right flex justify-end md:text-[30px] lg:text-[40px] hover:text-[#221115]">
                    <div>NoreBase Clone</div>
                </div>
                <div class="border-[1px] border-[#C1BEB8] w-full"></div>
                <div @mouseenter="showeasy()" @mouseleave="showeasy()"
                    class="font-[700] cursor-pointer mt-[48px] font-['panchang'] text-[24px] tx_stroke text-[transparent] text-right flex justify-end md:text-[30px] lg:text-[40px] hover:text-[#221115]">
                    <div>EasyBuddy Waitlist</div>
                </div>
                <div class="border-[1px] border-[#C1BEB8] w-full"></div>
                <div @mouseenter="showtred()" @mouseleave="showtred()"
                    class="font-[700] cursor-pointer mt-[48px] font-['panchang'] text-[24px] tx_stroke text-[transparent] text-right flex justify-end md:text-[30px] lg:text-[40px] hover:text-[#221115]">
                    <div>Tred Finance</div>
                </div>
            </div>
            <!--choose part-->
        </div>
    </div>
</template>

<style scoped>
.tx_stroke {
    -webkit-text-stroke: 1px #B3B3A3;
}
</style>
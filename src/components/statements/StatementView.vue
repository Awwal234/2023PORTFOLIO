<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    components: {
    },
    mounted() {

    },
    data() {
        return {

        }
    },
    methods: {

    },
});
</script>

<template>
    <div class="mt-[40.28px] md:mt-[113pxpx] px-[16px] md:px-[56px]">
        <div class="font-[400] leading-[24px] text-[12px] md:leading-[30px] text-[#8C8C8C] md:text-[20px]">
            Technology has had a profound impact on human progress, largely due to the emergence of digital technologies
            such as computers and software. Without the Ice Age, humanity could have advanced even further.This is whERE
            i COME IN, I LOVE BUILDING DIGITAL TECHNOLOGY SOLUTIONS THAT MOVES THE WORLD FROM HERE TO THERE!
        </div>
        <!-- ship to prod timeline -->
        <div class="md:flex md:space-x-[28px] md:items-stretch md:space-y-[] md:mt-[119px] mt-[72px] space-y-[24px]">
            <!--one ship-->
            <div class="border-[1px] w-full h-fit lg:h-[782px] md:w-[45%] border-[#C2BEB8] p-[16px]">
                <div
                    class="md:w-[214px] exec w-[214px] font-[600] text-[#221115] text-[] md:text-[24px] md:leading-[22px] leading-[20.8px]">
                    Executions with no strings Atta~ched
                </div>
                <div class="mt-[129px] w-fit h-fit md:mt-[61px]">
                    <img src="/img/carprod.png" class="w-[214px] h-[334px] md:h-[441px] md:w-[275px]" alt="" />
                </div>
                <div
                    class="w-full tracking-[-0.04em] md:w-fit font-['Panchang'] md:font-['Outfit'] mt-[32px] md:mt-[16px] font-[600] leading-[37px] md:leading-[74px] text-[#221115] text-[28px] md:text-[56px]">
                    SHIPT'O ~PROD
                </div>
                <div
                    class="mx-auto w-full md:w-[60%] text-center mt-[8px] font-[600] leading-[15.84px] md:leading-[18.48px] text-[#221115] text-[12px] md:text-[14px]">
                    From idea to iterating meet then to the path of execution and we ship like sailors☞⍣
                </div>
            </div>
            <!--end one ship-->
            <div class=" border-[#C2BEB8] lg:h-[782px] border-[1px]"></div>
            <!--second shipping-->
            <div class="w-full h-fit lg:h-[782px] tree md:w-[45%] p-[16px] md:px-[70px]">
                <div class="mt-[126px] mx-auto w-fit h-fit md:mt-[97px]">
                    <img src="/img/skate.png" class="w-[162px] skate h-[238px] md:w-[243px] md:h-[320px]" alt="" />
                </div>
                <div class="mt-[-90px] w-fit h-fit md:mt-[-120px]">
                    <img src="/img/alco.png" class="w-[162px] alco h-[238px] md:w-[243px] md:h-[320px]" alt="" />
                </div>
                <div class="flex relative mt-[-160px] md:mt-[-200px] justify-end w-full h-fit">
                    <div class="w-fit h-fit">
                        <img src="/img/hello.png" class="w-[162px] hello h-[238px] md:w-[243px] md:h-[320px]" alt="" />
                    </div>
                </div>
            </div>
            <!--end second shipping-->
        </div>
        <!-- end shipping to prod -->
    </div>
</template>

<style scoped>
.exec {
    font-family: 'Panchang', sans-serif;
}

.tree {
    background: url('/img/Treebg.png');
    background-repeat: no-repeat;
    background-position: cover;
    background-size: 100% 100%;
}

.skate {
    animation: 2s forwards cubic-bezier(0.075, 0.82, 0.165, 1) infinite skatel;
}

.alco {
    animation: 2s forwards cubic-bezier(0.075, 0.82, 0.165, 1) infinite alcol;
}

.hello {
    animation: 2s forwards cubic-bezier(0.075, 0.82, 0.165, 1) infinite hellol;
}

@keyframes skatel {
    10% {
        top: -1px;
        position: relative;
    }

    40% {
        top: -8px;
        position: relative;
    }

    60% {
        top: -15px;
        position: relative;
    }

    100% {
        top: 0px;
        position: relative;
    }
}

@keyframes alcol {
    10% {
        left: -1px;
        position: relative;
    }

    40% {
        left: -8px;
        position: relative;
    }

    60% {
        left: -15px;
        position: relative;
    }

    100% {
        left: 0px;
        position: relative;
    }
}

@keyframes hellol {
    10% {
        top: 1px;
        position: relative;
    }

    40% {
        top: 8px;
        position: relative;
    }

    60% {
        top: 15px;
        position: relative;
    }

    100% {
        top: 0px;
        position: relative;
    }
}
</style>
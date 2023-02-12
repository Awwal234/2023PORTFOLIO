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
    <div
        class="md:px-[56px] md:items-top space-y-[40px] md:space-y-[0px] md:space-x-[56px] mt-[59px] md:mt-[89px] md:flex px-[16px]">
        <!-- first slide -->
        <div class="w-full md:w-[50%] lg:w-[30%]">
            <div class="w-fit h-fit"><img src="/img/soilit.png" class="frame_one" alt="" /></div>
            <div class="mt-[8px] text-center md:text-left font-[600] text-[#221115] text-[14px] leading-[21px]">
                A son of the soil at ALTschool revolutionising the education system of Africa, per student, per time. A
                ground where with life’s are rescued.
            </div>
        </div>
        <!-- second slide -->
        <div class="line"></div>
        <!--third slide-->
        <div class="w-full md:w-[50%] lg:w-[25%]">
            <div
                class="font-[600] mx-auto frame_two md:mx-[0px] text-center text-[#221115] md:text-[48px] text-[48px] leading-[60.48px]">
                I AM HIM, NOT HYMN. FMD*
            </div>
            <div
                class="mt-[16px] md:mt-[12px] mx-auto text-center font-[600] text-[#221115] text-[14px] leading-[21px]">
                Creative Developer with sauce who has kept Nigeria relevant for the past 16 years and currently building
                for amazing brands looking to take the world a step further
            </div>
        </div>
        <!--fourth slide-->
        <div class="line md:hidden lg:block"></div>
        <!--fifth slide-->
        <div class="w-full md:hidden lg:w-[30%] lg:block">
            <div class="w-fit h-fit"><img src="/img/umbrellas.png" class="frame_three" alt="" /></div>
            <div class="mt-[8px] text-center md:text-right font-[600] text-[#221115] text-[14px] leading-[21px]">
                My adventures in life are purposefully created by the one who is beyond mortals and this makes it
                interesting for everyone like you to learn of.
            </div>
        </div>
        <!--end-->
    </div>
</template>

<style scoped>
.line {
    border: 1px solid #dddddd;
    background-image: linear-gradient(to right, #dddddd, #f2f2f2);
}

.frame_one {
    animation: forwards 2s cubic-bezier(0.075, 0.82, 0.165, 1) slide;
}

.frame_two {
    animation: moveDown 2s ease-in-out infinite;
}

.frame_three {
    animation: 2s ease-out forwards back;
}

@keyframes slide {
    10% {
        width: 5%;
    }

    30% {
        width: 40%;
    }

    60% {
        width: 60%
    }

    80% {
        width: 80%
    }

    100% {
        width: 100%;
    }
}

@keyframes back {
    10% {
        width: 5%;
    }

    30% {
        width: 40%;
    }

    60% {
        width: 60%
    }

    80% {
        width: 80%
    }

    100% {
        width: 100%;
    }

}

@keyframes moveDown {
    0% {
        transform: translateY(-20%);
        opacity: 1;
    }

    30% {
        transform: translateY(2%);
        top: 10px;
        position: relative;
        transform: rotate(1deg);
        opacity: 0.9;
    }

    100% {
        transform: translateY(40%);
        top: 10px;
        position: relative;
        transform: rotate(0deg);
        opacity: 0.5;
    }
}
</style>
<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    methods: {
        oncursor() {
            const arrow = document.getElementById('arrow') as HTMLDivElement
            const circle = document.getElementById('circle') as HTMLDivElement
            circle.classList.add('removearrow');
            arrow.classList.add('deletearrow');
            setTimeout((arrow.style.display = 'none'), 18000)
        },
        oncursorl() {
            const arrow = document.getElementById('arrowl') as HTMLDivElement
            const circle = document.getElementById('circlel') as HTMLDivElement
            circle.classList.add('removearrow');
            arrow.classList.add('deletearrow');
            setTimeout((arrow.style.display = 'none'), 18000)
        },
        notcursor() {
            const arrow = document.getElementById('arrow') as HTMLDivElement
            const circle = document.getElementById('circle') as HTMLDivElement
            circle.classList.remove('removearrow');
            arrow.classList.remove('deletearrow');
            arrow.style.display = 'block'
        },
        notcursorl() {
            const arrow = document.getElementById('arrowl') as HTMLDivElement
            const circle = document.getElementById('circlel') as HTMLDivElement
            circle.classList.remove('removearrow');
            arrow.classList.remove('deletearrow');
            arrow.style.display = 'block'
        },
        discoverenter() {
            const abt_me = document.getElementById('abt_me') as HTMLDivElement
            abt_me.classList.remove('abt_remove')
            abt_me.classList.add('abt_me')
        },
        discoverremove() {
            const abt_me = document.getElementById('abt_me') as HTMLDivElement
            abt_me.classList.remove('abt_me')
            abt_me.classList.add('abt_remove')
        },
        discoverenterl() {
            const abt_me = document.getElementById('abt_mel') as HTMLDivElement
            abt_me.classList.remove('abt_remove')
            abt_me.classList.add('abt_me')
        },
        discoverremovel() {
            const abt_me = document.getElementById('abt_mel') as HTMLDivElement
            abt_me.classList.remove('abt_me')
            abt_me.classList.add('abt_remove')
        },
    },
})
</script>

<template>
    <section class="md:mt-[128px] mt-[40px] md:px-[56px] px-[16px]">
        <div class="liney w-[90%] md:w-[90%] mx-auto h-[0px]"></div>
        <div class="mx-auto mt-[72px] md:mt-[88px] w-[80%] md:w-[80%]">
            <div class="font-[700] imc mx-auto text-[20px] text-right md:text-[72px] text-[#221115]">
                Imagine & Create
            </div>
            <div
                class="md:mt-[48px] flex justify-end text-[12px] md:text-[24px] leading-[24px] md:leading-[40px] tt text-[#221115] md:w-[100%] lg:w-[100%] text-right mt-[32px]">
                <div class="md:w-[80%] lg:w-[60%]">
                    Technology has had a profound impact on human progress, largely due to the emergence of digital
                    technologies such as computers and software. Without the Ice Age, humanity could have advanced even
                    further.
                </div>
            </div>
            <div
                class="md:mt-[48px] flex justify-end md:mb-[61px] text-[12px] md:text-[24px] leading-[24px] md:leading-[40px] tt text-[#221115] md:w-[100%] lg:w-[100%] mx-auto text-right mt-[32px]">
                <div class="md:w-[80%] lg:w-[60%]">
                    This is whERE i COME IN, I LOVE BUILDING DIGITAL TECHNOLOGY SOLUTIONS THAT MOVES THE WORLD FROM HERE
                    TO
                    THERE!
                </div>
            </div>
            <div
                class="md:mt-[80px] md:flex md:justify-end mb-[113px] w-fit h-fit hidden text-[12px] md:text-[24px] leading-[24px] md:leading-[40px] tt text-[#221115] md:w-[100%] lg:w-[100%] text-right mt-[45.72px]">
                <div class="w-[80%] h-fit space-x-[29.11px] flex items-center">
                    <div id="abt_me" @mouseenter="discoverenter()" @mouseleave="discoverremove()"
                        class="font-[700] w-full cursor-pointer imc text-right text-[14px] disc leading-[18px] text-[#221115] md:leading-[40px] md:text-[24px]">
                        DISCOVER MORE ABOUT ME
                    </div>
                    <div>
                        <div @mouseenter="oncursor()" @mouseleave="notcursor()" id="circle"
                            class="w-[48px] h-[48px] cursor-pointer absolute rounded-full border-[4.5px] border-[#221115]">
                        </div>
                        <div>
                            <img src="/img/arrow.svg" id="arrow" @mouseenter="oncursor()"
                                class="relative top-[15px] left-[0px] lg:left-[-8px]" alt="" />
                        </div>
                    </div>
                </div>
            </div>
            <!-- mobile more -->
            <div
                class="md:mt-[61px] md:hidden text-[12px] md:text-[24px] leading-[24px] md:leading-[40px] tt text-[#221115] md:float-right md:w-[90%] lg:w-[70%] text-right mt-[45.72px]">
                <div class="w-[100%] relative space-x-[29.11px] flex items-center">
                    <div id="abt_mel" @mouseenter="discoverenterl()" @mouseleave="discoverremovel()"
                        class="font-[700] w-full cursor-pointer imc text-right text-[14px] disc leading-[18px] text-[#221115] md:leading-[40px] md:text-[24px]">
                        MORE ABOUT ME
                    </div>
                    <div>
                        <div id="circlel" @mouseleave="notcursorl()" @mouseenter="oncursorl()"
                            class="w-[24.55px] h-[24.55px] cursor-pointer absolute rounded-full border-[2.3px] border-[#221115]">
                        </div>
                        <div id="arrowl" @mouseenter="oncursorl()"><img src="/img/arrowtwo.svg"
                                class="relative top-[8px] left-[-2px]" alt="" />
                        </div>
                    </div>
                </div>
            </div>
            <!-- emd more -->
        </div>
    </section>
</template>

<style scoped>
.liney {
    border: 1px solid #dddddd;
    background-image: linear-gradient(to right, #dddddd, #f2f2f2);
}

.imc {
    font-family: 'Panchang', sans-serif;
}

.tt {
    text-transform: uppercase;
}

.disc {
    text-decoration: underline;
}

.removearrow {
    animation: forwards 1s up;
}

@keyframes up {
    from {
        background: #E3E1DE;
        position: relative;
    }

    to {
        background: url('/img/eye.png');
        background-position: center;
        background-size: 32px 32px;
        background-repeat: no-repeat;
        position: relative;
    }
}

.deletearrow {
    animation: forwards 1s del;
}

@keyframes del {
    from {
        position: relative;
        top: -10px;
        left: 10px;
    }

    to {
        position: relative;
    }
}

.abt_me {
    animation: forwards 1s abt;
}

.abt_remove {
    animation: forwards 1s abtr;
}

@keyframes abt {
    from {
        position: relative;
        top: -20px;
    }

    to {
        position: relative;
        top: 0px;
        filter: blur(0px);
    }
}

@keyframes abtr {
    10% {
        position: relative;
        top: 20px;
    }

    50% {
        position: relative;
        opacity: 0;
        filter: blur(0px);
    }

    100% {
        position: relative;
        transform: translateY(-30%);
        top: 10px;
    }
}
</style>
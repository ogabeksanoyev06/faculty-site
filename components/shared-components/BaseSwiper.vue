<template>
  <div class="container max-w-screen-xl">
    <div class="w-full">
      <div class="relative">
        <div
          class="overflow-hidden px-[150px] -mx-[150px] md:py-1.5 md:-my-1.5 relative z-0"
        >
          <Swiper
            class="w-full !overflow-visible relative z-0"
            :modules="[SwiperAutoplay]"
            :slides-per-view="3"
            :loop="true"
            :autoplay="{
              delay: 8000,
              disableOnInteraction: true,
            }"
            :breakpoints="{
              475: {
                slidesPerView: 1,
                spaceBetween: 30,
              },
              576: {
                slidesPerView: 2,
                spaceBetween: 20,
              },
              960: {
                slidesPerView: 3,
                spaceBetween: 15,
              },
              1440: {
                slidesPerView: 3,
                spaceBetween: 10,
              },
            }"
          >
            <SwiperSlide v-for="slide in 10" :key="slide">
              <a
                href="https://edu.uz"
                target="_blank"
                class="flex items-center bg-white rounded px-2 py-4 border-b border-gray-400 hover:-translate-y-1 transition-all duration-500"
              >
                <div class="h-[50px] max-w-full flex-[0_0_50px] mr-4">
                  <img
                    src="https://innovation.gov.uz/media/interactive_services/cropped-oliy-talim-fan-va-innovatsiyalar-vazirligi-logo-01-01.png"
                    class="w-full h-full object-contain object-center"
                  />
                </div>
                <div class="text-xs font-medium line-clamp-3">
                  O‘zbekiston Respublikasi Oliy ta’lim, fan va innovatsiyalar
                  vazirligi
                </div>
              </a>
            </SwiperSlide>
          </Swiper>
          <div
            class="swiper-overlay absolute right-0 top-0 bottom-0 w-[228px] z-[1] pointer-events-none"
          />
          <div
            class="swiper-overlay rotate-180 absolute left-0 top-0 bottom-0 w-[228px] z-[1] pointer-events-none"
          />
        </div>

        <!-- <button
          class="bg-white hover:bg-blue hover:text-white -rotate-90 w-11 h-11 flex items-center justify-center shadow-card rounded-full transition-300 swiper-button sw-btn max-lg:-translate-x-full absolute right-0 translate-x-1/2 top-1/2 -translate-y-1/2 z-[3]"
          :class="{ 'opacity-100 !visible': showNextBtn }"
          aria-label="slide right"
          @click="slideNext"
        >
          <span class="icon-chevron text-lg">
            <svg
              width="20"
              height="20"
              viewBox="0 0 20 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M15.8334 7.5L10 13.3333L4.16669 7.5"
                stroke="#000"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </span>
          asass
        </button>
        <button
          class="bg-white hover:bg-blue hover:text-white rotate-90 w-11 h-11 flex items-center justify-center shadow-card rounded-full transition-300 swiper-button sw-btn max-lg:-translate-x-full absolute left-0 -translate-x-1/2 top-1/2 -translate-y-1/2 z-[3] sw-prev-el-0"
          :class="{ 'opacity-100 !visible': showPrevBtn }"
          aria-label="slide left"
          @click="slidePrev"
        >
          <span class="icon-chevron text-lg">
            <svg
              width="20"
              height="20"
              viewBox="0 0 20 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M15.8334 7.5L10 13.3333L4.16669 7.5"
                stroke="#000"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </span>
        </button> -->
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const slider = ref();
const showPrevBtn = ref(false);
const showNextBtn = ref(false);

const slidePrev = () => {
  slider.value.swiper.slidePrev();
};

const slideNext = () => {
  swiper.slideNext();
};
</script>

<style lang="scss" scoped>
.swiper-overlay {
  background: linear-gradient(90deg, #f5f6f700, #f5f6f7 97.58%);
}
</style>

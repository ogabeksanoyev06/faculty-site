<template>
  <div class="py-10 mt-10">
    <div class="container max-w-screen-xl">
      <BaseTitle title="Takliflar" />
      <div class="grid gap-5 grid-cols-1 md:grid-cols-2 lg:grid-cols-3">
        <div v-for="item in 4" :key="item">
          <div
            class="overflow-hidden rounded relative transition-all duration-300 cards"
          >
            <div class="absolute bottom-8 w-full z-10">
              <div
                class="flex items-center justify-between gap-2 px-8 relative after:absolute after:bg-white after:left-4 after:top-0 after:h-full after:w-[2px]"
              >
                <span
                  class="text-base sm:text-xl font-semibold text-white line-clamp-2 flex-1"
                >
                  Robototexnika kurslari endi bizda mavjud
                </span>
                <span
                  class="flex items-center justify-center w-8 h-8 bg-white rounded-full cursor-pointer"
                >
                  <svg
                    width="38"
                    height="38"
                    viewBox="0 0 38 38"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                    class="w-6 h-6"
                  >
                    <path
                      d="M25.3392 14.9058L11.7121 28.5329L9.47294 26.2938L23.1 12.6667H11.0892V9.5H28.5059V26.9167H25.3392V14.9058Z"
                      fill="#01193F"
                    />
                  </svg>
                </span>
              </div>
            </div>

            <img
              src="https://tsue.uz/media/video_gallery_thumbnails/tadbir_rasm.jpeg"
              class="w-full sm:h-full sm:object-cover"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import BaseTitle from "../shared-components/BaseTitle.vue";
</script>

<style lang="scss" scoped>
.cards::after {
  background: linear-gradient(0deg, rgba(3, 27, 64, 1), rgba(10, 32, 66, 0));
  bottom: 0;
  content: "";
  left: 0;
  position: absolute;
  right: 0;
  top: 0;
  transition: 0.5s ease-in-out;
  z-index: 1;
}
</style>

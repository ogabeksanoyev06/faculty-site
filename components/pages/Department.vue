<template>
  <div class="py-10 mt-10">
    <div class="container max-w-screen-xl">
      <BaseTitle title="Kafedralar" />
      <div
        class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-5"
      >
        <div
          class="flex items-center rounded bg-white border-b border-gray-400 p-3 gap-2 md:p-4 md:gap-3 max-md:justify-center max-md:flex-col cursor-pointer transition-all duration-300 hover:shadow-card hover:-translate-y-1 h-full"
          v-for="item in 6"
          :key="item"
        >
          <div class="w-8 h-8 preloader-image">
            <img
              src="https://cdn.commeta.uz/100x/https://cdn.commeta.uz/media/media/Group_MVewrf7.svg"
              alt="category-icon"
              class="w-full h-full"
            />
          </div>
          <div
            class="flex-grow flex flex-col max-md:text-center justify-between space-y-1"
          >
            <h3 class="text-xs md:text-sm font-medium">
              Suniyintelekt kafedrasi sadsdsd
            </h3>
            <p class="text-[11px] md:text-xs text-gray-400 w-full">
              674 ta O'qituvchilar
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import BaseTitle from "../shared-components/BaseTitle.vue";
</script>

<style lang="scss" scoped></style>

<template>
  <div class="py-10 mt-10 bg-gray-100">
    <div class="container max-w-screen-xl">
      <BaseTitle
        title="So'nggi yangiliklar"
        :btn="true"
        btnTitle="Barcha yangiliklar"
      />
      <div class="flex space-x-2 overflow-y-auto mini-x-scroll">
        <Button variant="default"> Active </Button>
        <Button variant="outline" v-for="(item, i) in newsTab" :key="i">
          {{ item.name }}
        </Button>
      </div>
      <div class="mt-5">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-5">
          <div
            class="flex flex-col sm:flex-row gap-2 shadow-[0_0_12px_3px_rgba(56,56,56,.05)] rounded overflow-hidden bg-white cursor-pointer hover:shadow-none hover:-translate-y-1 transition-all duration-500"
            v-for="(item, i) in 5"
            :key="i"
          >
            <div class="overflow-hidden">
              <img
                src="https://tmci.uz/files/common/newsproxy/News/photo_2024-02-09_14-40-47-2024-02-09_094230.jpg"
                alt=""
                class="object-top transition duration-700 ease-in-out sm:w-[250px] object-cover max-w-full"
              />
            </div>
            <div class="flex flex-col justify-between gap-1 py-4 px-2 flex-1">
              <div>
                <span
                  class="font-semibold text-primary text-base mb-1 leading-[130%] line-clamp-1"
                  >Yangiliklar</span
                >
                <p class="text-sm font-medium text-ellipsis line-clamp-3">
                  Toshkent davlat iqtisodiyot universitetida Birlashgan
                  Millatlar Tashkiloti Ayollar dasturining interaktiv muloqoti
                  o‘tkazildi.
                </p>
              </div>

              <div class="flex items-center gap-2">
                <p class="text-xs font-semibold text-primary leading-[130%]">
                  RI
                </p>
                <span class="w-[0.6px] h-[14px] bg-primary"></span>
                <Badge variant="secondary" class="rounded">02.03.2024</Badge>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import BaseTitle from "~/components/shared-components/BaseTitle";

const newsTab = [
  {
    id: 1,
    name: "Yangiliklar",
  },
  {
    id: 2,
    name: "E'lonlar",
  },
  {
    id: 3,
    name: "Tadbirlar",
  },
  {
    id: 4,
    name: "Tanlovlar",
  },
  {
    id: 5,
    name: "Jamiyat",
  },
];
</script>

<style lang="scss" scoped>
.scroll-mini::-webkit-scrollbar {
  height: 0;
}
</style>

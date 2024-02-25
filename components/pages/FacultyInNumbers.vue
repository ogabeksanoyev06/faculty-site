<template>
  <div class="py-10 mt-10 bg-gray-100">
    <div class="container max-w-screen-xl">
      <div class="">
        <h1 class="text-xl sm:text-2xl font-bold text-primary ">
          RAQAMLI IQTISODIYOT FAKULTETI
        </h1>
        <p class="text-xl sm:text-2xl text-primary">Raqamlarda</p>
      </div>
      <div
        class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 mt-5 gap-5"
      >
        <div
          class="flex flex-col justify-center items-center bg-white p-4 space-y-2 border-b rounded hover:shadow-[rgba(102,117,137,0.3)_0px_-1px_inset,rgba(18,28,37,0.07)_0px_4px_30px,rgba(18,28,37,0.06)_0px_3px_20px] transition-all duration-300"
          v-for="item in 4"
          :key="item"
        >
          <div class="w-16 h-16">
            <img
              src="https://cdn.commeta.uz/100x/https://cdn.commeta.uz/media/media/Group_hRAf0el.svg"
              alt="category-icon"
              class="w-full h-full"
            />
          </div>
          <Badge variant="secondary" class="rounded text-center">
            Magistr
          </Badge>
          <span class="text-2xl font-semibold">2800</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>

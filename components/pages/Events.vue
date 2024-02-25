<template>
  <div class="py-8 mt-8">
    <div class="container max-w-screen-xl">
      <BaseTitle
        title="Kutilayotgan tadbirlar"
        :btn="true"
        btnTitle="Barcha tadbirlar"
      />
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-5">
        <div
          class="flex flex-col gap-5 p-4 border rounded bg-white cursor-pointer hover:shadow-none hover:-translate-y-1 transition-all duration-300"
          v-for="(item, i) in 5"
          :key="i"
        >
          <div>
            <h2 class="text-base font-medium mb-4">
              <span class="text-primary" style="font-size: xx-large">23</span>
              - Fevral, Juma
            </h2>
            <h6 class="text-sm line-clamp-2 font-semibold text-ellipsis">
              Annaqulov Kamol Xasanovichning iqtisodiyot fanlari bo‘yicha
              falsafa doktori (PhD) dissertatsiya ishi himoyasi to‘g‘risida
            </h6>
          </div>
          <div class="">
            <div class="flex items-center justify-between flex-wrap">
              <p class="text-xs font-medium">
                <span class="font-semibold">RI</span> 02:00 - 04:00
              </p>
              <Badge variant="success" class="rounded"> Yakunlangan </Badge>
            </div>
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

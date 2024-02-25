<template>
  <div
    class="flex flex-col space-y-2 sm:flex-row items-center justify-between mb-10"
  >
    <div class="flex items-center gap-3">
      <i class="icon hidden sm:flex">
        <svg
          width="3"
          height="42"
          viewBox="0 0 3 42"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M0 0C1.65685 0 3 1.34315 3 3V39C3 40.6569 1.65685 42 0 42V0Z"
            fill="#010D21"
          ></path>
        </svg>
      </i>
      <h1 class="text-xl sm:text-2xl font-bold text-primary">{{ title }}</h1>
    </div>
    <Button variant="outline" class="group justify-between" v-if="btn">
      {{ btnTitle }}
      <img
        src="/assets/svg/angle-right.svg"
        alt=""
        class="group-hover:translate-x-2 transition-all duration-300"
      />
    </Button>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  title: String,
  btnTitle: String,
  routerLink: String,
  btn: {
    type: Boolean,
    default: false,
  },
});
</script>

<style lang="scss" scoped></style>

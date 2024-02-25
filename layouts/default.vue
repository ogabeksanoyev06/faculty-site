<template>
  <div>
    <AppHeader />
    <div class="overflow-x-hidden">
      <slot />
    </div>
  </div>
</template>

<script setup>
import AppHeader from "~/components/layouts/default/header/AppHeader.vue";
</script>

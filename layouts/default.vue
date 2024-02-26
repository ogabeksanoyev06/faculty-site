<template>
  <div>
    <AppHeader />
    <div class="overflow-x-hidden">
      <slot />
    </div>
    <AppFooter />
  </div>
</template>

<script setup>
import AppFooter from "~/components/layouts/default/footer/AppFooter.vue";
import AppHeader from "~/components/layouts/default/header/AppHeader.vue";
</script>

<template>
  <div>
    <HeroBanner />
    <FacultyInNumbers />
    <CtaBanner />

    <suggestions />
    <News />
    <Events />
    <Department />
    <UseFul />
  </div>
</template>

<script setup>
import CtaBanner from "~/components/pages/CtaBanner.vue";
import Department from "~/components/pages/Department.vue";
import Events from "~/components/pages/Events.vue";
import FacultyInNumbers from "~/components/pages/FacultyInNumbers.vue";
import HeroBanner from "~/components/pages/HeroBanner.vue";
import News from "~/components/pages/News.vue";
import Suggestions from "~/components/pages/Suggestions.vue";
import UseFul from "~/components/pages/UseFul.vue";
</script>

<style lang="scss" scoped></style>

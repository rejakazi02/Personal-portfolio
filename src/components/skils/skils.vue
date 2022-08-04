<script>
import skils from "../../data/skils";

export default {
  data: () => {
    return {
      skils,
    };
  },
};
</script>

<template>
  <!-- Projects grid -->
  <section class="pt-10 sm:pt-14">
    <!-- Projects grid title -->
    <div class="text-center mb-16">
      <p
        class="font-general-semibold text-2xl sm:text-5xl font-semibold mb-2 text-ternary-dark dark:text-ternary-light"
      >
        Skils
      </p>
    </div>

    <!-- Projects grid -->
    <div
      class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-12 mt-6 sm:gap-10 mx-20"
    >
      <div v-for="item in skils" :key="item.id" class="flex items-center justify-center flex-col">
        <img :src="item.img" alt="" />
        <h1 class="mt-4">{{ item.title }}</h1>
      </div>
    </div>
  </section>
</template>

<style scoped></style>

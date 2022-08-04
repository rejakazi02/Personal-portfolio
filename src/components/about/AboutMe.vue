<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'A motivated, passionate, responsible, strategic and enterprising young professional whose aim is to establish himself as a well renowned creative person through developing his knowledge by working in a well reputed organization, gather experiences of working in a team and gain the capability of leading team which will increase his confident and working skills and betterment for his future.',
				},
			],
		};
	},
};
</script>

<template>
  <div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
    <!-- About profile image -->
    <div class="w-full sm:w-1/4 mb-7 sm:mb-0">
      <img src="../../assets/images/1.png" class="rounded-xl w-96" alt="" />
    </div>

    <!-- About details -->
    <div class="w-full sm:w-3/4 text-left flex items-center">
      <p
        v-for="bio in bios"
        :key="bio.id"
        class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg text-justify"
      >
        {{ bio.bio }}
      </p>
    </div>
  </div>
</template>

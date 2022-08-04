<script>
export default {
  setup() {
    return {
      bios: [
        {
          id: 1,
          bio: "Hi, I am Reaj Morshed.",
        },
        {
          id: 2,
          bio: "A motivated, passionate, responsible, strategic and enterprising young professional whose aim is to establish himself as a well renowned creative person through developing his knowledge by working in a well reputed organization, gather experiences of working in a team and gain the capability of leading team which will increase his confident and working skills and betterment for his future.",
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
    <div class="w-full sm:w-3/4 text-left flex flex-col justify-center mt-20">
      <p
        v-for="bio in bios"
        :key="bio.id"
        class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg text-justify "
      >
        {{ bio.bio }}
      </p>

      <div class="flex flex-col items-center">
        <h1 class="pHeader mb-4">Personal Information</h1>
        <div class="personalDetails">
          <div class="flex flex-col items-end">
            <p>Name</p>
            <p>Father's Name</p>
            <p>Mother's Name</p>
            <p>Gender</p>
            <p>Date of Birth</p>
            <p>Blood Group </p>
            <p>Marital Status</p>
            <p>Nationality</p>
            <p>Religion</p>
            <p>Permanent Address</p>  <br>
            <p>Current Location</p>
            
            
          </div>
          <div class="flex flex-col items-center">
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p>
            <p class="font-black">:</p> <br>
            <p class="font-black">:</p>
            
          </div>

          <div class="flex flex-col items-start">
            <p>Reaj Morshed</p>
            <p>MD. Joynal Abedin</p>
            <p>Rina Akter</p>
            <p>Male</p>
            <p>December 20, 1996</p>
            <p>O+</p>
            <p>Unmarried</p>
            <p>Bangladeshi</p>
            <p>Islam</p>
            <p>Village: Dumuriya, Post: Pinjuri, Kotalipara, Kotalipara, Gopalganj</p> 
            <p> House No:2/1, Road No:4, Block No:F, Mirpur-2, Dhaka-1216</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

.personalDetails{
  display: grid;
  grid-template-columns: 1fr .3fr 1fr;
}

.pHeader{
  font-size: 24px;
    font-weight: 700;
    margin-left: 28px;
}


</style>
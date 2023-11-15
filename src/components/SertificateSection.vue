<template>
  <div class="container pt-[10px] xl:py-[100px]">
    <div class="wrapper flex items-center justify-center flex-col">
      <h1
        class="m-auto pb-[30px] text-[24px] text-[#1B1B35] font-bold xl:text-[40px]"
      >
        Sertifikatlar
      </h1>
      <div class="sertificates items-center justify-center border-none xl:flex">
        <div class="sertificate1 relative">
          <img
            src="/src/assets/images/mobile/sertificate1.png"
            class="w-[330px] xl:hidden"
            alt="#"
          />
          <img
            src="/src/assets/images/desktop/xl_sertification2.png"
            class="hidden xl:block"
            alt="#"
          />
        </div>
        <div class="sertificate2 relative">
          <img
            src="/src/assets/images/mobile/sercificate2.png"
            class="w-[330px] xl:hidden"
            alt="#"
          />
          <img
            src="/src/assets/images/desktop/xl_sertification.png"
            class="w-[556px] rounded-xl hidden xl:block"
            alt="#"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style scoped></style>

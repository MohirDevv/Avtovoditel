<template>
  <div class="container pt-[10px] xl:py-[100px]">
    <div class="wrapper flex items-center justify-center flex-col">
      <h1 class="m-auto pb-[30px] text-[24px] text-[#1B1B35] font-bold xl:text-[40px]">
        Sertifikatlar
      </h1>
      <div class="sertificates items-center justify-center border-none xl:flex">
        <div class="sertificate1 relative">
          <img
            src="/src/assets/images/mobile/sertificate1.png"
            class="w-[330px] xl:hidden"
            alt="#"
          />
          <img src="/src/assets/images/desktop/xl_sertification2.png" class="hidden xl:block" alt="#">
          <div
            class="backg m-auto w-[300px] h-[370px] hover:bg-[black] hover:bg-opacity-[50%] absolute inset-0 transition-all rounded xl:hidden"
            @click="isOpen = true"
          >
            <img
              src="/src/assets/icons/focus.svg"
              class="absolute top-[45%] right-[40%] opacity-0"
              alt="#"
            />
          </div>
        </div>
        <div class="sertificate2 relative">
          <img
            src="/src/assets/images/mobile/sercificate2.png"
            class="w-[330px] xl:hidden"
            alt="#"
          />
          <img src="/src/assets/images/desktop/xl_sertification.png" class="w-[556px] rounded-xl hidden xl:block" alt="#">
          <div
            class="backg m-auto w-[300px] h-[370px] hover:bg-[black] hover:bg-opacity-[50%] absolute inset-0 transition-all rounded xl:hidden"
            @click="isSecondOpen = true"
          >
            <img
              src="/src/assets/icons/focus.svg"
              class="absolute top-[45%] right-[40%] opacity-0"
              alt="#"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
  <teleport to="body">
    <div class="" v-if="isOpen">
      <div
        @click="isOpen = false"
        class="fixed inset-0 top-0 left-0 bottom-0 bg-[#00000099] z-[50]"
      ></div>
      <div
        class="fixed modal top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center flex-col z-[60] bg-white rounded-xl w-[330px] xl:w-[540px] xl:h-[650px] xl:bg-transparent"
        v-if="isOpen"
      >
        <button
          v-on:click="isOpen = !isOpen"
          class="absolute top-[-40px] right-[0%]"
        >
          <img src="/src/assets/icons/remove.svg" alt="plus" />
        </button>
        <img
          src="/src/assets/images/mobile/sertificate1.png"
          class="w-[330px] xl:hidden"
          alt="#"
        />
        <img src="/src/assets/images/desktop/xl_sertification2.png" class="hidden xl:block" alt="#">
      </div>
    </div>
  </teleport>
  <teleport to="body">
    <div class="" v-if="isSecondOpen">
      <div
        @click="isSecondOpen = false"
        class="fixed inset-0 top-0 left-0 bottom-0 bg-[#00000099] z-50"
      ></div>
      <div
        class="fixed modal top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center flex-col z-[60] bg-white rounded-xl w-[330px] xl:w-[540px] xl:h-[650px] xl:bg-transparent"
        v-if="isSecondOpen"
      >
        <button
          v-on:click="isSecondOpen = !isSecondOpen"
          class="absolute top-[-40px] right-[0%]"
        >
          <img src="/src/assets/icons/remove.svg" alt="plus" />
        </button>
        <img
          src="/src/assets/images/mobile/sercificate2.png"
          class="w-[330px] xl:hidden"
          alt="#"
        />
        <img src="/src/assets/images/desktop/xl_sertification.png" class="hidden xl:block" alt="#">
      </div>
    </div>
  </teleport>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      isSecondOpen: false,
    };
  },
};
</script>

<style scoped>
.backg:hover img{
  opacity: 1;
  transition: .3s;
}
</style>

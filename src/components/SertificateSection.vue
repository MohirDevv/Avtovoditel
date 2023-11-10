<template>
  <div class="container pt-[10px]">
    <div class="wrapper flex items-center justify-center flex-col">
      <h1 class="m-auto pb-[30px] text-[24px] text-[#1B1B35] font-bold">
        Sertifikatlar
      </h1>
      <div class="sertificates border-none">
        <div class="sertificate1">
          <img
            src="/src/assets/images/mobile/sertificate1.png"
            class="w-[330px]"
            alt="#"
            @click="isOpen = true"
          />
        </div>
        <div class="sertificate2">
          <img
            src="/src/assets/images/mobile/sercificate2.png"
            class="w-[330px]"
            alt="#"
            @click="isSecondOpen = true"
          />
        </div>
      </div>
    </div>
  </div>
  <teleport to="body">
    <div class="" v-if="isOpen">
      <div
        @click="isOpen = false"
        class="fixed inset-0 top-0 left-0 bottom-0 bg-[#00000099] z-[1]"
      ></div>
      <div
        class="fixed modal top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center flex-col z-[2] bg-white  rounded-xl w-[330px]"
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
            class="w-[330px]"
            alt="#"
          />
      </div>
    </div>
  </teleport>
  <teleport to="body">
    <div class="" v-if="isSecondOpen">
      <div
        @click="isSecondOpen = false"
        class="fixed inset-0 top-0 left-0 bottom-0 bg-[#00000099] z-[1]"
      ></div>
      <div
        class="fixed modal top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center flex-col z-[2] bg-white  rounded-xl w-[330px]"
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
            class="w-[330px]"
            alt="#"
          />
      </div>
    </div>
  </teleport>
</template>

<script>
export default {
  data() {
    return{
      isOpen: false,
      isSecondOpen: false,
    }
  }
};
</script>

<style scoped></style>

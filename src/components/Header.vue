<template>
  <div
    class="container pb-[54px] bg-[url('/src/assets/images/mobile/mobile-bg.png')] bg-cover bg-no-repeat"
  >
    <div class="wrapper flex items-center justify-center flex-col">
      <div class="content max-w-[360px]">
        <div class="entrImage">
          <img
            src="../assets/images/mobile/mobile_header.png"
            class=""
            alt="#"
          />
        </div>
        <div class="entrText">
          <h1 class="text-white text-[24px] font-black uppercase mb-[15px]">
            Hech qanday qo'rquv va stresslarsiz Mashina haydashni o'rganing!
          </h1>
          <div
            class="subbutton text-white flex justify-between border-[#FFFFFF1A] border-b-2 pb-[15px] mb-[20px]"
          >
            <p
              class="w-[190px] text-[14px] font-medium bg-[#D2E0FF1A] rounded-lg px-[15px] py-[5px]"
            >
              B kategoriyasi uchun boshlang'ich to'lov 1 160 000 so'mdan 0%
              nasiya
            </p>
            <p
              class="text-[14px] flex items-center justify-center font-medium bg-[#D2E0FF1A] rounded-lg px-[15px] py-[14px]"
            >
              Haftada 6 kun
            </p>
          </div>
        </div>
        <div
          class="iconsinfo1 flex items-center justify-between pb-[30px] pr-[30px]"
        >
          <div class="first">
            <img
              src="/src/assets/icons/calen.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p class="text-white text-[16px] font-semibold">
              XX yillik tajriba
            </p>
          </div>
          <div class="second">
            <img
              src="/src/assets/icons/user_options.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p class="text-white text-[16px] font-semibold">
              Eng yaxshi o'qitish usuli
            </p>
          </div>
        </div>
        <div
          class="iconsinfo2 flex items-center justify-between border-[#FFFFFF1A] border-b-2 pb-[20px] mb-[30px]"
        >
          <div class="first">
            <img
              src="/src/assets/icons/responsive.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p class="text-white text-[16px] font-semibold">Online format</p>
          </div>
          <div class="second">
            <img
              src="/src/assets/icons/home.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p class="text-white text-[16px] font-semibold">
              Toshkent bo'yicha 7 ta fillial
            </p>
          </div>
        </div>
        <div class="ariza flex items-center justify-center flex-col">
          <h2 class="text-[#FFFFFFE5] text-[12px] text-center pb-[10px]">
            Hoziroq ariza qoldiring va 10% chegirmaga ega bo'ling
          </h2>
          <button
            class="bg-[#407BFF] rounded-[50px] text-white px-[103px] py-[14px] mb-[20px] hover:bg-[#2C5AC2] transition-all"
            v-on:click="isOpen = true"
          >
            <p class="w-[115px]">Ariza qoldirish</p>
          </button>
        </div>
      </div>
      <h3
        class="w-[100%] max-w-[100%] text-[13px] text-center text-[#D8E1FF] font-medium bg-[#D2E0FF1A] py-[10px]"
      >
        Xonalarimiz eshiklari siz uchun ochiq
      </h3>
    </div>
  </div>
  <!-- <div
    class="fixed top-0 bottom-0 left-0 right-0 bg-black bg-opacity-[50%]"
    v-if="isOpen"
  >
    <div
      class="header_modal bg-white 2xl:w-[450px] w-[353px] h-[315px] mx-auto 2xl:h-[405px] 2xl:mt-[10%] mt-[234px] p-[20px] rounded-[12px] 2xl:py-[40px] 2xl:px-[30px] relative"
    >
      <button
        v-on:click="isOpen = !isOpen"
        class="absolute top-[-40px] right-0"
      >
        <img src="/src/assets/icons/remove.svg" alt="plus" />
      </button>

      <h1
        class="text-center 2xl:text-[24px] text-[20px] font-semibold mb-[3px]"
      >
        Telefon raqamingizni qoldiring
      </h1>
      <p
        class="text-center text-[#BABABA] 2xl:text-[18px] text-[16px] mb-[20px]"
      >
        Biz siz bilan albatta bog'lanamiz
      </p>
      <form>
        <input
          class="border-b-[1px] border-[#E0E0E0] w-full 2xl:mb-[50px] mb-[40px]"
          type="text"
          id="name"
          name="name"
          placeholder="Ism"
        />
        <input
          class="border-b-[1px] border-[#E0E0E0] w-full mb-[50px]"
          type="tel"
          id="tel"
          name="tel"
          placeholder="Raqamingiz"
        />
      </form>
      <button
        class="bg-[#407BFF] rounded-[50px] text-white px-[103px] py-[14px] mb-[20px] hover:bg-[#2C5AC2] transition-all"
      >
        <p class="w-[115px]">Ariza qoldirish</p>
      </button>
    </div>
  </div> -->

  <teleport to="body">
    <div class="" v-if="isOpen">
      <div
        @click="isOpen = false"
        class="fixed inset-0 top-0 left-0 bottom-0 bg-[#00000099] z-[1]"
      ></div>
      <div
        class="fixed modal top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center flex-col z-[2] bg-white p-[20px] rounded-xl"
        v-if="isOpen"
      >
        <button
          v-on:click="isOpen = !isOpen"
          class="absolute top-[-40px] right-[0%]"
        >
          <img src="/src/assets/icons/remove.svg" alt="plus" />
        </button>
        <h1
          class="text-center text-[22px] font-semibold mb-[3px]"
        >
          Telefon raqamingizni qoldiring
        </h1>
        <p
          class="text-center text-[#BABABA] text-[16px] mb-[20px]"
        >
          Biz siz bilan albatta bog'lanamiz
        </p>
        <form class="w-[310px]">
          <input
            class="border-b-[1px] border-[#E0E0E0] w-[300px] 2xl:mb-[50px] mb-[40px]"
            type="text"
            id="name"
            name="name"
            placeholder="Ism"
          />
          <input
            class="border-b-[1px] border-[#E0E0E0] w-[300px] mb-[50px]"
            type="tel"
            id="tel"
            name="tel"
            placeholder="Raqamingiz"
          />
        </form>
        <button
          class="bg-[#407BFF] rounded-[50px] text-white px-[103px] py-[14px] mb-[10px] hover:bg-[#2C5AC2] transition-all"
        >
          <p class="w-[115px]">Ariza qoldirish</p>
        </button>
      </div>
    </div>
  </teleport>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  mounted() {
    setTimeout(() => {
      this.isOpen = true;
    }, 1500);
  },
  methods: {},
};
</script>

<style scoped>

.modal {
  animation: fadeIn 0.7s;
  transition: 2s;
}
@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@media screen and (min-width: 440px) {
  .container {
    padding-bottom: 0px;
  }
}
</style>

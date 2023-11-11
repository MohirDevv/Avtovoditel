<template>
  <div
    class="container pb-[54px] bg-[url('/src/assets/images/mobile/mobile-bg.png')] bg-cover bg-no-repeat xl:relative overflow-x-hidden"
  >
    <div
      class="wrapper flex items-center justify-center flex-col xl:flex-row xl:relative overflow-x-hidden xl:justify-start"
    >
      <div
        class="content max-w-[360px] xl:max-w-[1100px] xl:pl-[150px] 2xl:pl-[250px] xl:pb-[113px]"
      >
        <div
          class="entrImage flex items-start justify-start relative pb-[10px] xl:pb-[62px] xl:pt-[20px]"
        >
          <img src="../assets/icons/avtovoditel_icon.svg" class="hidden xl:block" alt="#" />
          <img src="/src/assets/icons/car+symbol.svg" class="block xl:hidden" alt="">
          <img
            src="/src/assets/icons/last-symbol.png"
            class="absolute -top-5 -right-12 xl:hidden"
            alt="#"
          />
        </div>
        <div class="entrText">
          <h1
            class="text-white text-[24px] xl:text-[50px] font-black uppercase mb-[15px]"
          >
            Hech qanday qo'rquv va stresslarsiz Mashina haydashni o'rganing!
          </h1>
          <div
            class="subbutton text-white flex justify-between border-[#FFFFFF1A] border-b-2 pb-[15px] mb-[20px] xl:gap-[10px] xl:border-none xl:justify-normal"
          >
            <p
              class="w-[190px] xl:w-[660px] xl:flex xl:items-center text-[14px] font-medium bg-[#D2E0FF1A] xl:bg-[#407BFF] xl:text-[19px] xl:font-normal rounded-lg px-[15px] py-[5px]"
            >
              B kategoriyasi uchun boshlang'ich to'lov 1 160 000 so'mdan 0%
              nasiya
            </p>
            <p
              class="text-[14px] flex items-center justify-center font-medium bg-[#D2E0FF1A] rounded-lg px-[15px] py-[14px] xl:bg-[#407BFF] xl:text-[19px]"
            >
              Haftada 6 kun
            </p>
          </div>
        </div>
        <div
          class="iconsinfo1 flex items-center justify-between xl:justify-normal xl:gap-[30px] pb-[30px] pr-[30px]"
        >
          <div class="first xl:flex xl:items-center xl:gap-[15px]">
            <img
              src="/src/assets/icons/calen.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              XX yillik tajriba
            </p>
          </div>
          <div class="second xl:flex xl:items-center xl:gap-[15px]">
            <img
              src="/src/assets/icons/user_options.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Eng yaxshi o'qitish usuli
            </p>
          </div>
        </div>
        <div
          class="iconsinfo2 flex items-center justify-between border-[#FFFFFF1A] border-b-2 pb-[20px] mb-[30px] xl:justify-normal xl:gap-[40px] xl:border-none"
        >
          <div class="first xl:flex xl:items-center xl:gap-[15px]">
            <img
              src="/src/assets/icons/responsive.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Online format
            </p>
          </div>
          <div class="second xl:flex xl:items-center xl:gap-[15px]">
            <img
              src="/src/assets/icons/home.svg"
              class="bg-[#FFFFFF1A] rounded-[50%] p-[8px] mb-[8px]"
              alt="#"
            />
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Toshkent bo'yicha 7 ta fillial
            </p>
          </div>
        </div>
        <div
          class="ariza flex items-center justify-center flex-col xl:items-start"
        >
          <h2
            class="text-[#FFFFFFE5] text-[12px] text-center pb-[10px] xl:hidden"
          >
            Hoziroq ariza qoldiring va 10% chegirmaga ega bo'ling
          </h2>
          <button
            class="bg-[#407BFF] xl:bg-[#FFFFFF0D] rounded-[50px] text-white px-[103px] xl:px-0 py-[14px] xl:py-0 mb-[20px] hover:bg-[#2C5AC2] xl:hover:bg-[#FFFFFF0D] transition-all xl:flex xl:gap-3 xl:items-center"
            v-on:click="isOpen = true"
          >
            <p class="text-[20px] font-medium hidden px-[30px] xl:block">
              Hoziroq ariza qoldiring va 10% chegirmaga ega bo'ling
            </p>
            <p
              class="w-[115px] xl:w-[175px] xl:bg-[#407BFF] xl:rounded-[50px] xl:px-[30px] xl:py-[15px] xl:hover:bg-[#2C5AC2] transition-all"
            >
              Ariza qoldirish
            </p>
          </button>
        </div>
      </div>
      <div class="bigcar hidden xl:flex absolute bottom-0 right-0">
        <img src="/src/assets/icons/xlcar.svg" class="w-[350px] 2xl:w-[500px]" alt="#" />
      </div>
      <h3
        class="w-[100%] max-w-[100%] text-[13px] text-center text-[#D8E1FF] font-medium bg-[#D2E0FF1A] py-[10px] xl:hidden"
      >
        Xonalarimiz eshiklari siz uchun ochiq
      </h3>
    </div>
    <img
      src="/src/assets/icons/stop.svg"
      class="absolute bottom-[15%] left-[-50px] hidden xl:block"
      alt="#"
    />
    <img
      src="/src/assets/icons/go-on.svg"
      class="absolute top-[30%] right-[10%] hidden xl:block"
      alt="#"
    />
    <img
      src="/src/assets/icons/redsymbol.svg"
      class="absolute top-[-90px] right-[-70px] hidden xl:block"
      alt="#"
    />

    <p
      class="paragc text-[#D8E1FF] text-[20px] font-medium absolute bg-[#3d3c3c6b] rounded px-[20px] py-[10px] text-center hidden xl:block"
    >
      Xonalarimiz eshiklari siz uchun ochiq
    </p>
  </div>

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
        <h1 class="text-center text-[22px] font-semibold mb-[3px]">
          Telefon raqamingizni qoldiring
        </h1>
        <p class="text-center text-[#BABABA] text-[16px] mb-[20px]">
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
    }, 3000);
  },
  methods: {},
};
</script>

<style scoped>

.wrapper{
  max-width: 1980px;
}
.paragc{
  top: 0%;
  left: 50%;
  transform: translate(-50%, 0%);
}
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

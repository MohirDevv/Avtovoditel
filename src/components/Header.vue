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
            class="bg-[#407BFF] rounded-[50px] text-white px-[103px] py-[14px] mb-[20px] hover:bg-[#2C5AC2]
             transition-all"
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
</template>

<script>
export default {};
</script>

<style scoped>
@media screen and (min-width: 440px) {
  .container{
    padding-bottom: 0px;
  }
}
</style>

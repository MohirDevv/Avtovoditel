<template>
  <div class="container relative">
    <iframe
      src="https://yandex.com/map-widget/v1/?um=constructor%3A73748008eefd2cd0fdbedc588dbba1ae0eb1b1736568efbd69d5a4b876414713&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
    ></iframe>
    <div
      class="flex items-center justify-between w-[full] py-[10px] px-[15px] rounded-[6px] h-[65px] border-[1px] border-[#EAEAEA] relative top-[-72px] left-0 bg-white mx-[20px]"
     >
      <div class="flex items-center justify-between w-full ">
        <p class="text-[#1B1B35] text-[16px] font-medium cursor-pointer" v-on:click="isOpen = !isOpen">
          Filialni tanlang
        </p>
        <!-- <p class="text-[#1B1B35] text-[16px] font-medium" >
          Sergeli tumani Quruvchilar massivi 32 uy 1 qavat. Mo'ljal 305-maktab
        </p>
        <p class="text-[#808080] text-[18px] font-normal">
                Tel: 99 435 11 88
              </p> -->

        <button v-on:click="isOpen = !isOpen" class="block">
          <img src="/src/assets/icons/cheron-up.svg" alt="vec" class="cursor-pointer"
          :class="isOpen ? 'rotate-180 transition-all' : 'transition-all'"/>
        </button>
      </div>

      <div
        :class="isOpen ? 'block' : 'hidden'"
        class="scroll relative z-50 block top-[-897.5px] left-[-100%] "
      >
        <div
          class="w-[330px] bg-white rounded-[8px] border-[1px] border-[#EAEAEA] absolute top-[472px] left-[-15.5px] p-[10px] overflow-auto h-[400px]"
        >
          <div>
            <!-- <h1 class="text-[32px] font-bold mb-[20px]">Filiallar</h1> -->
            <div class="hoveroption border-b-[1px] border-[#EAEAEA] py-[15px] mb-[15px] hover:text-[#407BFF]">
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Sergeli tumani Quruvchilar massivi 32 uy 1 qavat. Mo'ljal
                305-maktab
              </h3>
              <p class="text-[#808080] text-[18px] font-normal ">
                Tel: 99 435 11 88
              </p>
            </div>
            <div class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px]">
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Tuzel chorraxa 2-qavat
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel 99 919 11 88
              </p>
            </div>
            <div class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px]">
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Panelniy massiv Oxangrabo ko'chasi
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 94 424 11 88
              </p>
            </div>
            <div class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px]">
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Mirzo Ulugbek tumani yalangoch daxasi Madaniyat instituti
                yaqinida
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 88 333 11 88
              </p>
            </div>
            <button
              class="flex justify-start flex-col hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px]"
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35] text-left">
                Yakkasaroy tumani Qushbegi daxasi 30 B uy. Oldingi Sulton
                restorani binosi 3 qavat
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 90 929 11 88
              </p>
            </button>
            <div class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px]">
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Sergeli tumani 6A 77 uy
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 99 710 05 55
              </p>
            </div>
            <div class="hoveroption pb-[15px] mb-[15px]">
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Tuzel - 1 50 uy
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 93 009 77 88
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      isChanged: false,
    };
  },
};
</script>

<style scoped>
/* Общие стили */
::-webkit-scrollbar {
  width: 12px; /* Ширина скроллбара */
}

::-webkit-scrollbar-thumb {
  background-color: #a0a0a0; /* Цвет ползунка */
  border-radius: 6px; /* Скругление углов ползунка */
}

::-webkit-scrollbar-track {
  background-color: #f0f0f0; /* Цвет фона дорожки */
  border-radius: 6px; /* Скругление углов дорожки */
}

.hoveroption:hover h3,
.hoveroption:hover p{
  color: #407BFF;
  transition: .3s;
}
</style>

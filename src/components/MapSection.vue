<template>
  <div class="container relative">
    <iframe
      src="https://yandex.com/map-widget/v1/?um=constructor%3A73748008eefd2cd0fdbedc588dbba1ae0eb1b1736568efbd69d5a4b876414713&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isDefault"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3A2b7f68146a437d5592bab59ec91b69de4eb88f9dca500bad09004fc0cde38ab8&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isSergili"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3Afd8beeab1d0cb1bfe3560f1ce52e51cc9c23c9b237bfc8fa26dd1e8e21dd80eb&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isTuzel"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3Aa6314e1f6a988f769c546b5089cd5c37d7606d8921a6a1fda8dafb166c193e3e&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isPanelniy"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3A712cb928f0706ac3748dda2eef0fbb9eb0a21377d0ff7fd6f6df4ca9cceb283b&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isYalongoch"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3A6c144da071997ec28b95fecbc7ed11268e290ea171413729a68e41ce6876c2ec&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isQushbegi"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3A47a421d807febb95145a71d97edac9179fba6b4667769d48bd8f179c39ed6d4c&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isSergili6a"
    ></iframe>
    <iframe
      src="https://yandex.ru/map-widget/v1/?um=constructor%3A72a37e0d51e2b7cacc67818054282b0fd412cb753a98ecd0ce6392aa0926c849&amp;source=constructor"
      width="100%"
      height="500"
      frameborder="0"
      class="z-10"
      v-if="isTuzel50"
    ></iframe>
    <div
      class="flex z-40 items-center justify-between w-[full] rounded-[6px] border-[1px] border-[#EAEAEA] relative top-[-72px] left-0 mx-[20px] xl:hidden"
    >
      <div
        class="flex items-center justify-between py-[10px] px-[15px] bg-white rounded-[6px] w-full z-40"
      >
        <p
          class="text-[#1B1B35] text-[16px] font-medium cursor-pointer"
          v-on:click="isOpen = !isOpen"
          v-if="isDefault"
        >
          Filialni tanlang
        </p>
        <div
          class="sergili cursor-pointer"
          v-if="isSergili"
          v-on:click="isOpen = !isOpen"
        >
          <p class="text-[#1B1B35] text-[16px] font-medium">
            Sergeli tumani Quruvchilar massivi 32 uy 1 qavat. Mo'ljal 305-maktab
          </p>
          <p class="text-[#808080] text-[18px] font-normal">
            Tel: 99 435 11 88
          </p>
        </div>
        <div
          class="Tuzel cursor-pointer"
          v-if="isTuzel"
          v-on:click="isOpen = !isOpen"
        >
          <h3 class="text-[18px] font-normal text-[#1B1B35]">
            Yashnobod tumani Tuzel chorraxa 2-qavat
          </h3>
          <p class="text-[#808080] text-[18px] font-normal">Tel 99 919 11 88</p>
        </div>
        <div
          class="Panelniy cursor-pointer"
          v-if="isPanelniy"
          v-on:click="isOpen = !isOpen"
        >
          <h3 class="text-[18px] font-normal text-[#1B1B35]">
            Yashnobod tumani Panelniy massiv Oxangrabo ko'chasi
          </h3>
          <p class="text-[#808080] text-[18px] font-normal">
            Tel: 94 424 11 88
          </p>
        </div>
        <div
          class="Yalongoch cursor-pointer"
          v-if="isYalongoch"
          v-on:click="isOpen = !isOpen"
        >
          <h3 class="text-[18px] font-normal text-[#1B1B35]">
            Mirzo Ulugbek tumani yalangoch daxasi Madaniyat instituti yaqinida
          </h3>
          <p class="text-[#808080] text-[18px] font-normal">
            Tel: 88 333 11 88
          </p>
        </div>
        <div
          class="Qushbegi cursor-pointer"
          v-if="isQushbegi"
          v-on:click="isOpen = !isOpen"
        >
          <h3 class="text-[18px] font-normal text-[#1B1B35] text-left">
            Yakkasaroy tumani Qushbegi daxasi 30 B uy. Oldingi Sulton restorani
            binosi 3 qavat
          </h3>
          <p class="text-[#808080] text-[18px] font-normal">
            Tel: 90 929 11 88
          </p>
        </div>
        <div
          class="Sergili6a cursor-pointer"
          v-if="isSergili6a"
          v-on:click="isOpen = !isOpen"
        >
          <h3 class="text-[18px] font-normal text-[#1B1B35]">
            Sergeli tumani 6A 77 uy
          </h3>
          <p class="text-[#808080] text-[18px] font-normal">
            Tel: 99 710 05 55
          </p>
        </div>
        <div
          class="Tuzel50 cursor-pointer"
          v-if="isTuzel50"
          v-on:click="isOpen = !isOpen"
        >
          <h3 class="text-[18px] font-normal text-[#1B1B35]">
            Yashnobod tumani Tuzel - 1 50 uy
          </h3>
          <p class="text-[#808080] text-[18px] font-normal">
            Tel: 93 009 77 88
          </p>
        </div>

        <button v-on:click="isOpen = !isOpen" class="block">
          <img
            src="/src/assets/icons/cheron-up.svg"
            alt="vec"
            class="cursor-pointer"
            :class="isOpen ? 'rotate-180 transition-all' : 'transition-all'"
          />
        </button>
      </div>

      <div
        :class="isOpen ? 'block' : 'hidden'"
        class="scroll relative z-10 block top-[-897.5px] left-[-97%] xl:left-[-99%]"
      >
        <div
          class="w-[330px] bg-white rounded-[8px] border-[1px] border-[#EAEAEA] absolute top-[461px] left-[-15.5px] p-[10px] overflow-auto h-[400px]"
        >
          <div>
            <!-- <h1 class="text-[32px] font-bold mb-[20px]">Filiallar</h1> -->
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] py-[15px] mb-[15px] hover:text-[#407BFF] cursor-pointer"
              @click="
                (isDefault = false),
                  (isSergili = true),
                  (isTuzel = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Sergeli tumani Quruvchilar massivi 32 uy 1 qavat. Mo'ljal
                305-maktab
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 99 435 11 88
              </p>
            </div>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = true),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Tuzel chorraxa 2-qavat
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel 99 919 11 88
              </p>
            </div>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = true),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Panelniy massiv Oxangrabo ko'chasi
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 94 424 11 88
              </p>
            </div>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = true),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Mirzo Ulugbek tumani yalangoch daxasi Madaniyat instituti
                yaqinida
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 88 333 11 88
              </p>
            </div>
            <button
              class="flex justify-start flex-col hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = true),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35] text-left">
                Yakkasaroy tumani Qushbegi daxasi 30 B uy. Oldingi Sulton
                restorani binosi 3 qavat
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 90 929 11 88
              </p>
            </button>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = true),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Sergeli tumani 6A 77 uy
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 99 710 05 55
              </p>
            </div>
            <div
              class="hoveroption pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = true),
                  (isOpen = false)
              "
            >
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
    <!--  -->
    <!--  -->
    <!--  -->
    <div
      class="xl:flex z-40 items-center justify-between w-[full] rounded-[6px] border-[1px] border-[#EAEAEA] relative top-[-72px] left-0 mx-[20px] hidden"
    >

      <div
        class="scroll z-10 block"
      >
        <div
          class="w-[550px] bg-white rounded-[8px] border-[1px] border-[#EAEAEA] absolute bottom-[-40px] 
          left-[10px] p-[30px]"
        >
          <div>
            <h1 class="text-[32px] font-bold">Filiallar</h1>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] py-[15px] mb-[15px] hover:text-[#407BFF] cursor-pointer"
              @click="
                (isDefault = false),
                  (isSergili = true),
                  (isTuzel = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Sergeli tumani Quruvchilar massivi 32 uy 1 qavat. Mo'ljal
                305-maktab
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 99 435 11 88
              </p>
            </div>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = true),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Tuzel chorraxa 2-qavat
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel 99 919 11 88
              </p>
            </div>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = true),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Yashnobod tumani Panelniy massiv Oxangrabo ko'chasi
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 94 424 11 88
              </p>
            </div>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = true),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Mirzo Ulugbek tumani yalangoch daxasi Madaniyat instituti
                yaqinida
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 88 333 11 88
              </p>
            </div>
            <button
              class="flex justify-start flex-col hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = true),
                  (isSergili6a = false),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35] text-left">
                Yakkasaroy tumani Qushbegi daxasi 30 B uy. Oldingi Sulton
                restorani binosi 3 qavat
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 90 929 11 88
              </p>
            </button>
            <div
              class="hoveroption border-b-[1px] border-[#EAEAEA] pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = true),
                  (isTuzel50 = false),
                  (isOpen = false)
              "
            >
              <h3 class="text-[18px] font-normal text-[#1B1B35]">
                Sergeli tumani 6A 77 uy
              </h3>
              <p class="text-[#808080] text-[18px] font-normal">
                Tel: 99 710 05 55
              </p>
            </div>
            <div
              class="hoveroption pb-[15px] mb-[15px] cursor-pointer"
              @click="
                (isDefault = false),
                  (isTuzel = false),
                  (isSergili = false),
                  (isPanelniy = false),
                  (isYalongoch = false),
                  (isQushbegi = false),
                  (isSergili6a = false),
                  (isTuzel50 = true),
                  (isOpen = false)
              "
            >
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
      isDefault: true,
      isSergili: false,
      isTuzel: false,
      isPanelniy: false,
      isYalongoch: false,
      isQushbegi: false,
      isSergili6a: false,
      isTuzel50: false,
    };
  },
};
</script>

<style scoped>
::-webkit-scrollbar {
  width: 12px;
}

::-webkit-scrollbar-thumb {
  background-color: #a0a0a0;
  border-radius: 6px;
}

::-webkit-scrollbar-track {
  background-color: #f0f0f0;
  border-radius: 6px;
}

.hoveroption:hover h3,
.hoveroption:hover p {
  color: #407bff;
  transition: 0.3s;
}

@media screen and (min-width: 1280px) {
  iframe{
    height: 862px;
  }
}

</style>

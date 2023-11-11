<template>
  <div class="container bg-white py-[50px] xl:py-[150px]">
    <div class="wrapper flex items-center justify-center flex-col">
      <h1 class="text-[#1B1B35] text-[24px] font-bold xl:text-[40px]">
        Narxlarlar
      </h1>
      <div
        class="priceOption flex items-center justify-center gap-6 mt-[23px] p-[2px] bg-[#F3F3F3] rounded-lg xl:mb-[42px]"
      >
        <h2
          class="text-[14px] leading-4 cursor-pointer"
          :class="isNaqd ? 'active' : 'deactivated'"
          @click="oylikToNaqd"
        >
          Naqt to'lash
        </h2>
        <h2
          class="deactivated text-[14px] leading-4 cursor-pointer"
          :class="isOylik ? 'active' : 'deactivated'"
          @click="naqtToOylik"
        >
          Bo'lib to'lash
        </h2>
      </div>
      <div
        class="cardlist flex items-center justify-center flex-col py-[20px] xl:mb-[50px]"
      >
        <div
          class="cardLevel1 flex items-center justify-center gap-3 pb-[12px]"
        >
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg gap-4 p-[7px] sm:p-[15px]"
          >
            <h1
              class="h1 bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[4px] px-[15px] xl:text-[40px] xl:px-[22px] xl:py-[6px]"
            >
              B
            </h1>
            <p
              class="mainp text-[#1B1B35] text-[22px] font-semibold xl:text-[34px]"
              v-if="isNaqd"
            >
              2 900 000
            </p>
            <p
              class="subp w-[140px] text-center text-[14px] text-[#808080]"
              v-if="isOylik"
            >
              Boshlangich o'qish summasi 40% qolgani 90 kun ichida, o'qish
              davomiyligi 4 oy 20 kun
            </p>

            <img
              src="/src/assets/icons/b_class_car.svg"
              class="car xl:hidden"
              alt="#"
            />
            <img
              src="/src/assets/icons/b_classxl.svg"
              class="hidden xl:block"
              alt="#"
            />

            <button
              class="button border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[200px] xl:text-[18px]"
            >
              Kursni tanlash
            </button>
          </div>
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px]"
            :class="isOylik ? ' gap-[31px]' : 'gap-4'"
          >
            <h1
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[7px] px-[8px] xl:text-[40px] xl:px-[22px] xl:py-[6px]"
            >
              BC
            </h1>
            <p
              class="text-[#1B1B35] text-[22px] font-semibold xl:text-[34px]"
              v-if="isNaqd"
            >
              3 500 000
            </p>
            <p
              class="w-[140px] text-center text-[14px] text-[#808080]"
              v-if="isOylik"
            >
              Boshlangich o'qish summasi 1 000 000, oq'ish davomiyligi 6 oy
            </p>
            <div class="images flex gap-1 xl:hidden">
              <img src="/src/assets/icons/bc_class_car.svg" alt="#" />
              <img src="/src/assets/icons/b_class_car_sm.svg" alt="#" />
            </div>
            <img
              src="/src/assets/icons/bc_classxl.png"
              class="hidden xl:block"
              alt=""
            />
            <button
              class="border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[200px] xl:text-[18px]"
            >
              Kursni tanlash
            </button>
          </div>
        </div>
        <div class="cardLevel2 flex items-center justify-center gap-3">
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px]"
            :class="isOylik ? ' gap-[31px]' : 'gap-[15px]'"
          >
            <h1
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[4px] px-[15px] xl:text-[40px] xl:px-[22px] xl:py-[6px]"
            >
              C
            </h1>
            <p
              class="text-[#1B1B35] text-[22px] font-semibold xl:text-[34px]"
              v-if="isNaqd"
            >
              1 300 000
            </p>
            <p
              class="w-[140px] text-center text-[14px] text-[#808080]"
              v-if="isOylik"
            >
              Boshlangich o'qish summasi 45%, o'qish davomiyligi 3 oy
            </p>
            <img
              src="/src/assets/icons/c_class_car.svg"
              class="xl:hidden"
              alt="#"
            />
            <img
              src="/src/assets/icons/c_classxl.svg"
              class="hidden xl:block"
              alt="#"
            />
            <button
              class="border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[100px] xl:text-[18px]"
            >
              Kursni tanlash
            </button>
          </div>
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px]"
            :class="isOylik ? ' gap-[29px]' : 'gap-[15px]'"
          >
            <h1
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[7px] px-[16px] xl:text-[40px] xl:px-[22px] xl:py-[6px]"
            >
              D
            </h1>
            <p
              class="text-[#1B1B35] text-[22px] font-semibold xl:text-[34px]"
              v-if="isNaqd"
            >
              3 100 000
            </p>
            <p
              class="w-[140px] text-center text-[14px] text-[#808080]"
              v-if="isOylik"
            >
              Boshlangich o'qish summasi 45%, o'qish davomiyligi 3 oy
            </p>
            <img
              src="/src/assets/icons/d_class_car.svg"
              class="xl:hidden"
              alt="#"
            />
            <img
              src="/src/assets/icons/d_classxl.svg"
              class="hidden xl:block"
              alt="#"
            />
            <button
              class="border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[110px] xl:text-[18px]"
            >
              Kursni tanlash
            </button>
          </div>
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border xl:flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px] hidden"
            :class="isOylik ? ' gap-[35px]' : 'gap-[15px]'"
          >
            <h1
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[4px] px-[15px] hover:text-[white] xl:text-[40px] xl:px-[22px] xl:py-[6px]"
            >
              E
            </h1>
            <p
              class="text-[#1B1B35] text-[22px] font-semibold xl:text-[34px]"
              v-if="isNaqd"
            >
              1 500 000
            </p>
            <p
              class="w-[170px] text-center text-[14px] text-[#808080]"
              v-if="isOylik"
            >
              50% dan 2 oy, o'qish davomiyligi 2 oy
            </p>
            <img
              src="/src/assets/icons/e_class_car.svg"
              class="xl:hidden"
              alt="#"
            />
            <img
              src="/src/assets/icons/e_classxl.svg"
              class="hidden xl:block"
              alt="#"
            />
            <button
              class="border-[#E0E0E0] border-[2px] px-[24px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[110px] xl:text-[18px]"
            >
              <p class="">Kursni tanlash</p>
            </button>
          </div>
        </div>
        <div
          class="cardLevel3 flex items-center justify-center pt-[12px] w-[330px] xl:hidden"
        >
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg gap-4 p-[7px] sm:p-[15px]"
          >
            <h1
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[4px] px-[15px] hover:text-[white]"
            >
              E
            </h1>
            <p class="text-[#1B1B35] text-[22px] font-semibold" v-if="isNaqd">
              1 500 000
            </p>
            <p
              class="w-[170px] text-center text-[14px] text-[#808080]"
              v-if="isOylik"
            >
              50% dan 2 oy, o'qish davomiyligi 2 oy
            </p>
            <img src="/src/assets/icons/e_class_car.svg" alt="#" />
            <button
              class="border-[#E0E0E0] border-[2px] px-[24px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer"
            >
              <p class="w-[275px]">Kursni tanlash</p>
            </button>
          </div>
        </div>
      </div>
      <button
        class="bg-[#407BFF] rounded-[50px] text-white px-[113px] py-[14px] mb-[20px] hover:bg-[#2C5AC2] transition-all"
        v-on:click="isOpen = true"
      >
        <p class="w-[115px]">Ariza qoldirish</p>
      </button>
    </div>
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
      isNaqd: true,
      isOylik: false,
      isOpen: false,
    };
  },
  methods: {
    naqtToOylik() {
      if ((this.isNaqd = true)) {
        this.isNaqd = false;
        this.isOylik = true;
      }
    },
    oylikToNaqd() {
      if ((this.isOylik = true)) {
        this.isNaqd = true;
        this.isOylik = false;
      }
    },
  },
};
</script>

<style scoped>
.active {
  background: #ffffff;
  padding: 6px 12px;
  box-shadow: 0px 3px 1px 0px rgba(0, 0, 0, 0.04),
    0px 3px 8px 0px rgba(0, 0, 0, 0.12);
  border: 0.5px solid rgba(40, 41, 49, 0.04);
  border-radius: 6px;
  width: 150px;
  text-align: center;
  color: #407bff;
  font-weight: 600;
  transition: 0.3s;
}

.deactivated {
  text-align: center;
  padding: 6px 12px;
  width: 150px;
  transition: 0.3s;
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

@media screen and (min-width: 1280px) {
  .active {
    background: #ffffff;
    padding: 7px 13px;
    box-shadow: 0px 3px 1px 0px rgba(0, 0, 0, 0.04),
      0px 3px 8px 0px rgba(0, 0, 0, 0.12);
    border: 0.5px solid rgba(40, 41, 49, 0.04);
    border-radius: 6px;
    width: 150px;
    text-align: center;
    color: #407bff;
    font-weight: 600;
    transition: 0.3s;
  }

  .deactivated {
    text-align: center;
    padding: 7px 13px;
    width: 150px;
    transition: 0.3s;
  }
}

/* .card:hover .h1,
.card:hover .mainp,
.card:hover,
.card:hover .car,
.card:hover .button,
.card:hover .subp {
  color: white;
  background: #407bff;
  transition: .03s;
}
.card:hover .h1 {
  background: rgba(255, 255, 255, 0.1);
  transition: .03s;
}
.card:hover .car {
  background-color: #407bff;
  filter: brightness(-0) invert(-11);
  fill: #ffffff;
  background: #407bff;
} */
</style>

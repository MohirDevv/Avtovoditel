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
              class="subp w-[140px] text-center text-[14px] text-[#808080] xl:w-[336px]"
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
            <!-- <img
              src="/src/assets/icons/b_classxl.svg"
              
              alt="#"
            /> -->
            <svg
              width="150"
              height="72"
              viewBox="0 0 150 72"
              class="car1 hidden xl:block"
              fill="#1B1B35"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M21.0371 47.5503C25.6898 47.5503 29.4742 51.3037 29.4742 55.9157C29.4742 60.5285 25.6898 64.2804 21.0371 64.2804C16.3853 64.2804 12.6001 60.5285 12.6001 55.9157C12.6001 51.3037 16.3853 47.5503 21.0371 47.5503Z"
              />
              <path
                d="M4.81348 55.9156C4.81348 64.7985 12.0767 72.0001 21.0371 72.0001C29.9969 72.0001 37.2601 64.7985 37.2601 55.9156C37.2601 47.0327 29.9969 39.8311 21.0371 39.8311C12.0774 39.8311 4.81348 47.0327 4.81348 55.9156ZM8.99361 55.9156C8.99361 49.3318 14.3963 43.9754 21.0371 43.9754C27.678 43.9754 33.0807 49.3318 33.0807 55.9156C33.0807 62.4995 27.6787 67.8559 21.0371 67.8559C14.3956 67.8559 8.99361 62.4995 8.99361 55.9156Z"
              />
              <path
                d="M124.038 47.5503C128.69 47.5503 132.475 51.3037 132.475 55.9157C132.475 60.5285 128.69 64.2804 124.038 64.2804C119.386 64.2804 115.601 60.5285 115.601 55.9157C115.6 51.3037 119.385 47.5503 124.038 47.5503Z"
              />
              <path
                d="M107.815 55.9156C107.815 64.7985 115.078 72.0001 124.039 72.0001C132.998 72.0001 140.262 64.7985 140.262 55.9156C140.262 47.0327 132.998 39.8311 124.039 39.8311C115.078 39.8311 107.815 47.0327 107.815 55.9156ZM111.995 55.9156C111.995 49.3318 117.398 43.9754 124.039 43.9754C130.679 43.9754 136.081 49.3318 136.081 55.9156C136.081 62.4995 130.679 67.8559 124.039 67.8559C117.398 67.8559 111.995 62.4995 111.995 55.9156Z"
              />
              <path
                d="M0 37.8087V57.8655H2.92211C2.92211 57.8655 0 37.8087 21.0365 37.8087C42.073 37.8087 40.0117 57.8655 40.0117 57.8655H105.65C105.65 57.8655 103.402 37.5855 124.037 37.5855C144.673 37.5855 142.29 57.8655 142.29 57.8655H148.359C156.677 34.9117 131.051 24.8818 123.408 23.991C115.766 23.0995 88.1172 3.71098 76.8777 1.70545C65.6381 -0.300085 35.2919 -1.41486 21.0372 3.48845C6.78256 8.39104 6.07012 33.5744 6.07012 33.5744L0 37.8087ZM126.804 27.9157C126.804 27.9157 134.686 29.1886 140.26 34.5142C140.261 34.5142 126.57 38.7968 126.804 27.9157ZM64.4539 5.93313C67.9017 6.15418 71.0711 6.43013 73.7164 6.73169C88.933 8.46787 109.057 25.8326 109.057 25.8326H64.4547V5.93313H64.4539ZM30.8268 6.51578C38.9161 5.28537 50.3048 5.2334 60.2502 5.70038V25.8326H30.8268V6.51578ZM13.3126 25.8326C13.3126 25.8326 15.6478 16.1087 20.9021 10.0892C21.9977 8.83387 24.2746 7.88232 27.3244 7.17526V25.8319L13.3126 25.8326Z"
              />
            </svg>

            <button
              class="button border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[200px] xl:text-[18px]"
              v-on:click="onSelect('b')"
            >
              Kursni tanlash
            </button>
          </div>
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px]"
            :class="isOylik ? ' gap-[16.5px]' : 'gap-4'"
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
              class="w-[140px] text-center text-[14px] text-[#808080] xl:w-[336px]"
              v-if="isOylik"
            >
              Boshlangich o'qish summasi 1 000 000, oq'ish davomiyligi 6 oy
            </p>
            <div class="images flex gap-1 xl:hidden">
              <img src="/src/assets/icons/bc_class_car.svg" alt="#" />
              <img src="/src/assets/icons/b_class_car_sm.svg" alt="#" />
            </div>
            <img
              src="/src/assets/icons/bc_classxl.svg"
              class="hidden xl:block"
              alt=""
            />
            <button
              class="button border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[200px] xl:text-[18px]"
              v-on:click="onSelect('bc')"
            >
              Kursni tanlash
            </button>
          </div>
        </div>
        <div
          class="cardLevel2 flex items-center justify-center gap-3 xl:pt-[12px]"
        >
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px]"
            :class="isOylik ? ' gap-[29px]' : 'gap-[15px]'"
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
              class="w-[140px] text-center text-[14px] text-[#808080] xl:w-[336px]"
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
              class="button border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[100px] xl:text-[18px]"
              v-on:click="onSelect('c')"
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
              class="w-[140px] text-center text-[14px] text-[#808080] xl:w-[336px]"
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
              class="button border-[#E0E0E0] border-[2px] px-[22px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[110px] xl:text-[18px]"
              v-on:click="onSelect('d')"
            >
              Kursni tanlash
            </button>
          </div>
          <div
            class="card bg-[#FFFFFF] border-[#E0E0E0] border xl:flex items-center justify-center flex-col rounded-lg p-[7px] sm:p-[15px] hidden"
            :class="isOylik ? ' gap-[35.5px]' : 'gap-[15px]'"
          >
            <h1
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[4px] px-[15px] xl:text-[40px] xl:px-[22px] xl:py-[6px]"
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
              class="w-[170px] text-center text-[14px] text-[#808080] xl:w-[336px]"
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
              class="button border-[#E0E0E0] border-[2px] px-[24px] py-[12px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer xl:px-[110px] xl:text-[18px]"
              v-on:click="onSelect('e')"
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
              class="bg-[#E0E0E0] rounded-[50px] text-[24px] text-[#1B1B35] font-medium py-[4px] px-[15px]"
            >
              E
            </h1>
            <p class="text-[#1B1B35] text-[22px] font-semibold" v-if="isNaqd">
              1 500 000
            </p>
            <p
              class="w-[170px] text-center text-[14px] text-[#808080] xl:w-[336px]"
              v-if="isOylik"
            >
              50% dan 2 oy, o'qish davomiyligi 2 oy
            </p>
            <img src="/src/assets/icons/e_class_car.svg" alt="#" />
            <button
              class="button border-[#E0E0E0] border-[2px] px-[15px] py-[10px] rounded-lg text-[14px] text-[#1B1B35] font-medium cursor-pointer"
              v-on:click="onSelect('e')"
            >
              <p class="w-[275px]">Kursni tanlash</p>
            </button>
          </div>
        </div>
      </div>
      <button
        class="bg-[#407BFF] rounded-[50px] text-white px-[113px] py-[14px] mb-[20px] hover:bg-[#2C5AC2] transition-all"
        v-on:click="onSelect('body')"
      >
        <p class="w-[115px]">Ariza qoldirish</p>
      </button>
    </div>
  </div>

  <teleport to="body">
    <div class="" v-if="isOpen">
      <div
        @click="isOpen = false"
        class="fixed inset-0 top-0 left-0 bottom-0 bg-[#00000099] z-[9999]"
      ></div>
      <div
        class="fixed modal top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center flex-col z-[99999] bg-white p-[20px] rounded-xl"
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
            id="validator_name"
            placeholder="Ism"
            v-model="name"
            @input="formatNameValue()"
          />
          <input
            class="border-b-[1px] border-[#E0E0E0] w-[300px] mb-[50px]"
            type="tel"
            id="validator_num"
            placeholder="Raqamingiz"
            v-model="phone"
            @focus="onFocus()"
            @input="formatPhoneNumber()"
          />
        </form>
        <button
          class="bg-[#407BFF] rounded-[50px] text-white px-[103px] py-[14px] mb-[10px] hover:bg-[#2C5AC2] transition-all"
          @click="sendData"
        >
          <p class="w-[115px]">Ariza qoldirish</p>
        </button>
      </div>
    </div>
  </teleport>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      isNaqd: true,
      isOylik: false,
      isOpen: false,
      isValidNum: null,
      isVAlidName: null,
      phone: null,
      name: null,
      info1: "",
      isDataSent: false,
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
    formatPhoneNumber() {
      const num = document.getElementById("validator_num");
      let inputValue = this.phone
        .replace(/\D/g, "")
        .replace("9", "")
        .replace("9", "")
        .replace("8", "");

      if (inputValue.length > 9) {
        inputValue = inputValue.substring(0, 9);
      }

      if (inputValue.length <= 2) {
        this.phone = "+998 " + inputValue;
        num.classList.add("invalid");
      } else if (inputValue.length <= 5) {
        this.phone =
          "+998 " + inputValue.substring(0, 2) + " " + inputValue.substring(2);
      } else if (inputValue.length <= 7) {
        this.phone =
          "+998 " +
          inputValue.substring(0, 2) +
          " " +
          inputValue.substring(2, 5) +
          "-" +
          inputValue.substring(5);
        num.classList.add("invalid");
      } else {
        this.phone =
          "+998 " +
          inputValue.substring(0, 2) +
          " " +
          inputValue.substring(2, 5) +
          "-" +
          inputValue.substring(5, 7) +
          "-" +
          inputValue.substring(7, 9);
        num.classList.add("invalid");
        this.isValidNum = false;
      }

      if (inputValue.length == 9) {
        num.classList.remove("invalid");
        this.isValidNum = true;
      }
    },
    formatNameValue() {
      const name = document.getElementById("validator_name");
      let inputValue = this.name;
      if (inputValue.length == 0) {
        name.classList.add("invalid");
        this.isVAlidName = false;
      } else if (inputValue.length >= 1) {
        name.classList.remove("invalid");
        this.isVAlidName = true;
      }
    },
    onSelect(val) {
      this.isOpen = true;
      switch (val) {
        case "e":
          this.info1 = "Narxlar bloki, E";
          break;
        case "d":
          this.info1 = "Narxlar bloki, D";
          break;
        case "c":
          this.info1 = "Narxlar bloki, C";
          break;
        case "bc":
          this.info1 = "Narxlar bloki, BC";
          break;
        case "b":
          this.info1 = "Narxlar bloki, B";
          break;
        case "body":
          this.info1 = "Narxlar bloki";
          break;
        default:
          break;
      }
    },
    onFocus() {
      if (!this.phone) {
        this.phone = "+998 ";
      }
    },
    sendData() {
      const body = {
        name: this.name,
        phone_number: this.phone.replaceAll("-", "").replaceAll(" ", ""),
        project: "avtovoditel",
        info: this.info1,
      };

      if (
        this.isVAlidName !== true ||
        this.isValidNum !== true ||
        this.isVAlidName == null ||
        this.isValidNum == null
      ) {
        const name = document.getElementById("validator_name");
        const num = document.getElementById("validator_num");

        num.classList.add("invalid");
        name.classList.add("invalid");
      } else if (this.isValidNum == true && this.isVAlidName == true) {
        const name = document.getElementById("validator_name");
        const num = document.getElementById("validator_num");

        num.classList.remove("invalid");
        name.classList.remove("invalid");
        this.isDataSent = true;
        setTimeout(() => {
          this.isOpen = false;
          this.phone = "";
          this.name = "";
          this.info1 = "";
        }, 3000);
        setTimeout(() => {
          this.isDataSent = false;
        }, 2000);
        console.log("success");
        axios
          .post("https://crm.redapp.uz/api/customer/", body)
          .then((response) => {
            console.log(response);
          })
          .catch((error) => {
            console.log(error);
            if (error) {
              alert("Xato!");
              this.phone = "";
              this.name = "";
              this.info1 = "";
            }
          });
      }
    },
  },
  mounted() {},
};
</script>

<style scoped>
.invalid {
  border-bottom: 1px solid rgba(251, 74, 74, 0.4);
  /* background: rgba(255, 138, 138, 0.1); */
}
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

.button:hover {
  color: #ffffff;
  border: 2px solid #ffffff;
  background: #407bff;
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

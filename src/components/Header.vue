<template>
  <div
    class="container pb-[54px] bg-[url('/src/assets/images/mobile/mobile-bg.png')] bg-cover bg-no-repeat xl:relative overflow-x-hidden"
  >
    <div
      class="wrapper flex items-center justify-center flex-col xl:flex-row xl:relative overflow-x-hidden xl:justify-start"
    >
      <div
        class="content max-w-[360px] xl:max-w-[1100px] xl:pl-[110px] 2xl:pl-[250px] xl:pb-[30px] 3xl:pb-[80px]"
      >
        <div
          class="entrImage flex items-start justify-start relative pb-[10px] xl:pb-[32px] xl:pt-[20px]"
        >
          <div
            class="logo flex items-center justify-center gap-[10px] xl:mt-0 mt-[25px]"
          >
            <img
              src="../assets/icons/logo.svg"
              class="w-[55px] h-[55px] xl:w-[80px] xl:h-[80px]"
              alt="#"
            />
            <h1 class="text-white text-[16px] xl:text-[24px] font-extrabold">
              AVTOVODITEL
            </h1>
          </div>
        </div>
        <div class="entrText">
          <h1
            class="max-w-[800px] text-white text-[24px] xl:text-[50px] font-black uppercase mb-[15px]"
          >
            Hech qanday qo'rquv va stresslarsiz Mashina haydashni o'rganing!
          </h1>
          <div class="xl:pb-[50px] xl:flex pb-[20px]">
            <div
              class="rounded-t-[8px] border-b-[1px] border-[#455674] py-[10px] px-[15px] bg-[#323E55] xl:border-none xl:rounded-lg xl:bg-[#407BFF] xl:mr-[10px]"
            >
              <p class="font-medium text-[14px] text-white">
                B kategoriyasi uchun boshlang'ich to'lov 1 000 000 so'mdan 0%
                nasiya
              </p>
            </div>
            <div
              class="rounded-b-[8px] py-[10px] px-[15px] bg-[#323E55] xl:rounded-lg xl:bg-[#407BFF]"
            >
              <p class="font-medium text-[14px] text-white">Haftada 3 kun</p>
            </div>
          </div>
        </div>
        <div
          class="iconsinfo1 flex items-center justify-between xl:justify-normal xl:gap-[30px] pb-[30px] pr-[30px] xl:pr-0"
        >
          <div class="first xl:flex xl:items-center xl:gap-[15px] xl:pr-[12px]">
            <div
              class="img-bg flex items-center justify-center bg-[#FFFFFF1A] rounded-[50%] w-[40px] h-[40px] mb-[8px]"
            >
              <img src="/src/assets/icons/calen.svg" class="p-[8px]" alt="#" />
            </div>
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              5 yillik tajriba
            </p>
          </div>
          <div class="second xl:flex xl:items-center xl:gap-[15px]">
            <div
              class="img-bg flex items-center justify-center bg-[#FFFFFF1A] rounded-[50%] w-[40px] h-[40px] mb-[8px]"
            >
              <img
                src="/src/assets/icons/user_options.svg"
                class="p-[8px]"
                alt="#"
              />
            </div>
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Eng yaxshi o'qitish usuli
            </p>
          </div>
        </div>
        <div
          class="iconsinfo2 flex items-center justify-between pb-[20px] xl:justify-normal xl:gap-[40px]"
        >
          <div class="first xl:flex xl:items-center xl:gap-[15px]">
            <div
              class="img-bg flex items-center justify-center bg-[#FFFFFF1A] rounded-[50%] w-[40px] h-[40px] mb-[8px]"
            >
              <img
                src="/src/assets/icons/responsive.svg"
                class="p-[8px]"
                alt="#"
              />
            </div>
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Online format
            </p>
          </div>
          <div class="second xl:flex xl:items-center xl:gap-[15px]">
            <div
              class="img-bg flex items-center justify-center bg-[#FFFFFF1A] rounded-[50%] w-[40px] h-[40px] mb-[8px]"
            >
              <img src="/src/assets/icons/home.svg" class="p-[8px]" alt="#" />
            </div>
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Toshkent bo'yicha 10 ta fillial
            </p>
          </div>
        </div>
        <div
          class="iconsinfo3 flex items-center justify-between border-[#FFFFFF1A] border-b-2 pb-[20px] mb-[30px] xl:justify-normal xl:gap-[40px] xl:border-none"
        >
          <div
            class="third xl:flex xl:items-center xl:gap-[15px] justify-center"
          >
            <div
              class="img-bg flex items-center justify-center bg-[#FFFFFF1A] rounded-[50%] w-[40px] h-[40px] mb-[8px]"
            >
              <img
                src="/src/assets/icons/world-wide.svg"
                class="p-[8px]"
                alt="#"
              />
            </div>
            <p
              class="text-white text-[16px] xl:text-[20px] xl:font-medium font-semibold"
            >
              Darslar rus va o'zbek tilida bo'lib o'tadi
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
            v-on:click="onSelect('main')"
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
        <img
          src="/src/assets/icons/xlcar.svg"
          class="w-[400px] 2xl:w-[500px] 3xl:w-[770px]"
          alt="#"
        />
      </div>
      <div
        class="div flex items-center justify-center w-[100%] max-w-[100%] bg-[#D2E0FF1A] py-[10px] mb-[6px] xl:hidden"
      >
        <h3 class="text-[13px] text-center text-[#D8E1FF] font-medium">
          Xonalarimiz eshiklari siz uchun ochiq
        </h3>
      </div>
    </div>
    <div class="entroptions absolute mt-[19px] hidden xl:block">
      <div
        class="options flex gap-10 bg-[#FFFFFF1A] py-[15px] px-[30px] rounded-full border-[#515359] border"
      >
        <p
          class="text-white hover:text-[#407BFF] transition-all cursor-pointer"
          @click="scrollToPrice"
        >
          Narxlar
        </p>
        <p
          class="text-white hover:text-[#407BFF] transition-all cursor-pointer"
          @click="scrollToMap"
        >
          Filiallar
        </p>
      </div>
    </div>
    <img
      src="/src/assets/icons/stop.svg"
      class="absolute bottom-[15%] left-[-50px] hidden xl:block"
      alt="#"
    />
    <img
      src="/src/assets/icons/redsymbol.svg"
      class="absolute top-[-90px] right-[-70px] hidden xl:block"
      alt="#"
    />

    <p
      class="paragc text-[#D8E1FF] text-[20px] font-medium absolute bg-[#FFFFFF1A] px-[20px] py-[10px] text-center hidden xl:block"
    >
      Xonalarimiz eshiklari siz uchun ochiq
    </p>
    <div
      id="pagetop"
      class="fixed right-[10px] bottom-[10px] xl:right-[20px] xl:bottom-[20px] z-[999] transition-all cursor-pointer"
      v-show="scY > 300"
      @click="toTop"
    >
      <img
        src="/src/assets/icons/cheron-upwh.svg"
        class="bg-[#407BFF] rounded-xl p-1 xl:p-3"
        alt="#"
      />
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
        <form class="">
          <div class="input-container mt-[20px]">
            <input
              class="border-b-[1px] border-[#E0E0E0] w-[300px] 2xl:mb-[50px] mb-[40px]"
              type="text"
              id="name"
              v-model="name"
              @input="formatNameValue()"
              required
            />
            <label for="name">Ism</label>
          </div>

          <div class="input-container h-[50px]">
            <input
              class="border-b-[1px] border-[#E0E0E0] w-[300px] mb-[50px]"
              type="tel"
              id="number"
              v-model="phone"
              @focus="onFocus()"
              @input="formatPhoneNumber()"
              required
            />
            <label for="number">Raqamingiz</label>
          </div>
          <div
            class="dropdown flex items-center justify-between transition-all bg-[#e0e0e0] hover:bg-[#c1c1c1] rounded-lg mb-[10px] p-[10px] w-[300px]"
            @click.prevent="toggleDropdown"
          >
            <button class="dropdown-button flex justify-between items-center">
              {{ selectedOption || "Filial" }}
            </button>
            <img
              src="/src/assets/icons/dropdown-arrow.svg"
              alt="#"
              class="w-[20px] h-[24px] transition-all"
              :class="arrowRotationClass"
            />
            <div v-if="isDropdownOpen" class="dropdown-options">
              <ul class="h-[210px] overflow-auto">
                <li
                  v-for="(option, index) in dropdownOptions"
                  :key="index"
                  @click="selectOption(option)"
                >
                  {{ option }}
                </li>
              </ul>
            </div>
          </div>
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
import Swal from "sweetalert2";
export default {
  data() {
    return {
      isOpen: false,
      scTimer: 0,
      scY: 0,
      phone: null,
      name: null,
      info2: "Pop-up,",
      isValidNumber: null,
      isValiddName: null,
      isDataSentHeader: false,
      isDropdownOpen: false,
      selectedOption: null,
      dropdownOptions: [
        " Sergeli tumani Quruvchilar massivi 32 uy 1 qavat. Mo'ljal 305-maktab",
        " Yashnobod tumani Tuzel chorraxa 2-qavat",
        " Yashnobod tumani Panelniy massiv Oxangrabo ko'chasi",
        " Mirzo Ulugbek tumani yalangoch daxasi Madaniyat instituti yaqinida",
        " Yakkasaroy tumani Qushbegi daxasi 30 B uy. Oldingi Sulton restorani binosi 3 qavat",
        " Sergeli tumani 6A 77 uy",
        " Yashnobod tumani Tuzel - 1 50 uy",
        " M.Ulugbek tumani Qora-suv 2 Doniyor kochasi 2 berk",
        " Angren shaxri Duken qorgoni Visol toyxonasi oldida",
      ],
    };
  },
  mounted() {
    setTimeout(() => {
      this.isOpen = true;
    }, 3000);
    window.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    scrollToPrice() {
      const priceElement = document.getElementById("price");
      if (priceElement) {
        priceElement.scrollIntoView({
          behavior: "smooth", // Optional for smooth scrolling
        });
      }
    },
    scrollToMap() {
      const mapElement = document.getElementById("map");
      if (mapElement) {
        mapElement.scrollIntoView({
          behavior: "smooth", // Optional for smooth scrolling
        });
      }
    },
    handleScroll: function () {
      if (this.scTimer) return;
      this.scTimer = setTimeout(() => {
        this.scY = window.scrollY;
        clearTimeout(this.scTimer);
        this.scTimer = 0;
      }, 100);
    },
    toTop: function () {
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },
    onSelect(val) {
      this.isOpen = true;
      switch (val) {
        case "main":
          this.info2 = "Asosiy blok";
          break;
        default:
          break;
      }
    },
    formatPhoneNumber() {
      const num = document.getElementById("number");
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
        this.isValidNumber = false;
      }

      if (inputValue.length == 9) {
        num.classList.remove("invalid");
        this.isValidNumber = true;
      }
    },
    formatNameValue() {
      const name = document.getElementById("name");
      let inputValue = this.name;
      if (inputValue.length == 0) {
        name.classList.add("invalid");
        this.isValiddName = false;
      } else if (inputValue.length >= 1) {
        name.classList.remove("invalid");
        this.isValiddName = true;
      }
    },
    onFocus() {
      if (!this.phone) {
        this.phone = "+998 ";
      }
    },
    sendData() {
      if (!this.selectedOption) {
        alert("Filialni tanlang!");
      } else {
        const body = {
          name: this.name,
          phone_number: this.phone.replaceAll("-", "").replaceAll(" ", ""),
          info: this.info2 + this.selectedOption,
          project: "avtovoditel",
        };
        if (
          this.isValiddName !== true ||
          this.isValidNumber !== true ||
          this.isValiddName == null ||
          this.isValidNumber == null
        ) {
          const name = document.getElementById("name");
          const num = document.getElementById("number");

          num.classList.add("invalid");
          name.classList.add("invalid");
        } else if (this.isValidNumber == true && this.isValiddName == true) {
          const name = document.getElementById("name");
          const num = document.getElementById("number");

          num.classList.remove("invalid");
          name.classList.remove("invalid");
          this.isOpen = false;
          this.isDataSentHeader = true;
          if (this.isDataSentHeader == true) {
            Swal.fire({
              icon: "success",
              title: "Arizangiz qabul qilindi)",
              showConfirmButton: false,
              iconColor: "#407BFF",
              timer: 2000,
            });
          }
          setTimeout(() => {
            this.phone = "";
            this.name = "";
          }, 2000);
          setTimeout(() => {
            this.isDataSentHeader = false;
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
                this.phone = "";
                this.name = "";
                alert("Xato!");
              }
            });
        }
      }
    },
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
    },
    selectOption(option) {
      this.selectedOption = option;
    },
  },
  computed: {
    arrowRotationClass() {
      return this.isDropdownOpen ? "rotate-0" : "rotate-180";
    },
  },
};
</script>

<style scoped>
.input-container {
  position: relative;
}

label {
  position: absolute;
  top: 20%;
  left: 10px;
  transform: translateY(-50%);
  pointer-events: none;
  transition: 0.3s;
  color: #bababa;
}

input:focus + label,
input:valid + label {
  top: -10px;
  font-size: 12px;
  color: #407bff;
}
.invalid {
  border-bottom: 1px solid rgba(251, 74, 74, 0.4);
}
.wrapper {
  max-width: 1980px;
}
.paragc {
  width: 400px;
  bottom: 33%;
  left: 83%;
  transform: translate(-50%, 0%);
  border-radius: 16px 16px 0px 16px;
}
.entroptions {
  top: 0;
  left: 50%;
  transform: translate(-50%, 0%);
}
.modal {
  animation: fadeIn 0.7s;
  transition: 2s;
}

#pagetop {
  animation: fadeIn 0.7s;
  transition: 2s;
}
.dropdown {
  position: relative;
  /* display: inline-block; */
}

.dropdown-options {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 999;
  background-color: #ffffff;
  border: 1px solid #e0e0e0;
  border-radius: 4px;
  overflow: hidden;
}

.dropdown-options ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.dropdown-options li {
  padding: 10px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.dropdown-options li:hover {
  background-color: #f0f0f0;
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

@media screen and (min-width: 1536px) {
  .paragc {
    width: 400px;
    bottom: 38%;
    left: 84%;
    transform: translate(-50%, 0%);
    border-radius: 16px 16px 0px 16px;
  }
}
@media screen and (min-width: 1920px) {
  .paragc {
    width: 400px;
    bottom: 52%;
    left: 85.6%;
    transform: translate(-50%, 0%);
    border-radius: 16px 16px 0px 16px;
  }
}
</style>

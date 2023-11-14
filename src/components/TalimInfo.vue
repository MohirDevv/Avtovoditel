<template>
  <div class="container bg-white py-[50px] xl:py-[150px]">
    <div class="wrapper flex items-center justify-center flex-col">
      <h1 class="text-[#1B1B35] text-[24px] font-bold pb-[30px] animated-text">
        TA'LIM BOSQICHLARI
      </h1>
      <div
        class="iconsAnim flex items-center justify-center flex-col xl:hidden"
      >
        <div class="level1 flex items-center justify-center">
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/lamp.svg" alt="#" />
            <img
              src="/src/assets/icons/right-arrow.svg"
              class="bg-[#407BFF] p-[8px] rounded-[50px]"
              alt="#"
            />
            <p class="text-[#1B1B35] text-[18px]">Nazariy kurs</p>
          </div>
          <div
            class="text-[#E0E0E0] text-[30px] mt-[20px]"
            id="animated1"
            :class="{ line1: isVisible }"
          >
            - - - - - -
          </div>
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/triogonometry.svg" alt="#" />
            <img
              src="/src/assets/icons/down-arrow.svg"
              class="bg-[#E0E0E0] p-[8px] rounded-[50px]"
              :class="{ downArrow: isVisible }"
              alt="#"
            />
            <p class="text-[#1B1B35] text-[18px]">Amaliy kurs</p>
          </div>
        </div>
        <div
          class="text-[#E0E0E0] text-[30px] flex items-end justify-end mt-[40px] ml-[230px] rotate-90"
          :class="{ line2: isVisible }"
        >
          - - - - - -
        </div>
        <div class="level1 flex items-center justify-center mt-[35px]">
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/nurce.svg" alt="#" />
            <img
              src="/src/assets/icons/check-circle.svg"
              class="bg-[#E0E0E0] p-[8px] rounded-[50px]"
              alt="#"
              :class="{ leftArrow: isVisible }"
            />
            <p class="text-[#1B1B35] text-[18px]">YHXX imtihoni</p>
          </div>
          <div
            class="text-[#E0E0E0] text-[30px] mt-[20px]"
            :class="{ line3: isVisible }"
          >
            - - - - - -
          </div>
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/done_job.svg" alt="#" />
            <img
              src="/src/assets/icons/left-arrow.svg"
              class="bg-[#E0E0E0] p-[8px] rounded-[50px]"
              alt="#"
              :class="{ done: isVisible }"
            />
            <p class="text-[#1B1B35] text-[18px]">Ichki imtihon</p>
          </div>
        </div>
      </div>
      <div
        class="iconsAnim1 hidden xl:flex items-center justify-center flex-row"
      >
        <div class="level1 flex items-center justify-center">
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/lamp.svg" alt="#" />
            <img
              src="/src/assets/icons/right-arrow.svg"
              class="bg-[#407BFF] p-[8px] rounded-[50px]"
              alt="#"
            />
            <p class="text-[#1B1B35] text-[18px]">Nazariy kurs</p>
          </div>
          <div
            class="text-[#E0E0E0] text-[30px] mt-[20px] xl:mt-[15px]"
            id="animated"
            :class="{ line1: isVisible }"
          >
            - - - - - - - - -
          </div>
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/triogonometry.svg" alt="#" />
            <img
              src="/src/assets/icons/down-arrow.svg"
              class="bg-[#E0E0E0] p-[8px] rounded-[50px] xl:-rotate-90"
              :class="{ downArrow: isVisible }"
              alt="#"
            />
            <p class="text-[#1B1B35] text-[18px]">Amaliy kurs</p>
          </div>
        </div>
        <div
          class="text-[#E0E0E0] text-[30px] flex items-end justify-end mt-[35px] xl:mt-[15px] ml-[230px] xl:ml-[0] rotate-90 xl:rotate-0"
          :class="{ line2: isVisible }"
        >
          - - - - - - - - -
        </div>
        <div
          class="level1 flex items-center justify-center mt-[35px] xl:mt-0 xl:flex-row-reverse"
        >
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/nurce.svg" alt="#" />
            <img
              src="/src/assets/icons/check-circle.svg"
              class="bg-[#E0E0E0] p-[8px] rounded-[50px]"
              alt="#"
              :class="{ done: isVisible }"
            />
            <p class="text-[#1B1B35] text-[18px]">YHXX imtihoni</p>
          </div>
          <div
            class="text-[#E0E0E0] text-[30px] mt-[20px] xl:mt-[15px]"
            :class="{ line3: isVisible }"
          >
            - - - - - - - - -
          </div>
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/done_job.svg" alt="#" />
            <img
              src="/src/assets/icons/right-arrow.svg"
              class="bg-[#E0E0E0] p-[8px] rounded-[50px]"
              alt="#"
              :class="{ leftArrow: isVisible }"
            />
            <p class="text-[#1B1B35] text-[18px]">Ichki imtihon</p>
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
      isVisible: false,
    };
  },
  mounted() {
    this.isVisible = this.isElementInViewport();
    document.addEventListener("scroll", () => {
      if (!this.isVisible) {
        this.isVisible = this.isElementInViewport();
      }
    });
  },
  methods: {
    isElementInViewport() {
      const el = document.getElementById("animated");
      const el1 = document.getElementById("animated1");
      if (!el || !el1) return;

      var rect = el.getBoundingClientRect();
      var rect1 = el1.getBoundingClientRect();

      return (
        rect.top >= 0 &&
        rect1.top >= 0 &&
        rect.left >= 0 &&
        rect1.left >= 0 &&
        rect.bottom <=
          (window.innerHeight || document.documentElement.clientHeight) &&
        rect1.bottom <=
          (window.innerHeight || document.documentElement.clientHeight) &&
        rect.right <=
          (window.innerWidth || document.documentElement.clientWidth) &&
        rect1.right <=
          (window.innerWidth || document.documentElement.clientWidth)
      );
    },
  },
};
</script>

<style scoped>
.animated-text {
  animation: colorChange 2s;
  background: linear-gradient(to right, #e0e0e0, #1b1b35);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  display: inline-block;
  animation-fill-mode: forwards;
}

@keyframes colorChange {
  0% {
    color: #e0e0e0;
  }
  100% {
    color: #1b1b35;
  }
}

.line1 {
  animation: colorChangeLine 2s;
  background: linear-gradient(to right, #e0e0e0, #407bff);
  background-clip: text;
  background-size: 200% 100%;
  -webkit-background-clip: text;
  color: transparent;
  display: inline-block;
  animation-fill-mode: forwards;
}

@keyframes colorChangeLine {
  0% {
    background-position: 0% 0%;
    color: #e0e0e0;
  }
  100% {
    background-position: 100% 0%;
    color: #407bff;
  }
}

.downArrow {
  animation: colorChangeDown 2s;
  animation-fill-mode: forwards;
  animation-delay: 1s;
}

@keyframes colorChangeDown {
  0% {
    background: #e0e0e0;
  }
  100% {
    background: #407bff;
  }
}

.line2 {
  animation: colorChangeLine2 2s;
  color: linear-gradient(to right, #e0e0e0, #407bff);
  animation-fill-mode: forwards;
  animation-delay: 1.5s;
}

@keyframes colorChangeLine2 {
  0% {
    color: #e0e0e0;
  }
  100% {
    color: #407bff;
  }
}

.done {
  animation: colorChangeDown 2s;
  animation-fill-mode: forwards;
  animation-delay: 2.5s;
}

@keyframes colorChangeDown {
  0% {
    background: #e0e0e0;
  }
  100% {
    background: #407bff;
  }
}

.line3 {
  animation: colorChangeLine3 2s;
  color: linear-gradient(to right, #e0e0e0, #407bff);
  animation-fill-mode: forwards;
  animation-delay: 3.5s;
}

@keyframes colorChangeLine3 {
  0% {
    color: #e0e0e0;
  }
  100% {
    color: #407bff;
  }
}

.leftArrow {
  animation: colorChangeDown 2s;
  animation-fill-mode: forwards;
  animation-delay: 4.5s;
}
</style>

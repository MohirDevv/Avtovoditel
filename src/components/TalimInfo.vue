<template>
  <div class="container bg-white py-[50px]">
    <div class="wrapper flex items-center justify-center flex-col">
      <h1 class="text-[#1B1B35] text-[24px] font-bold pb-[30px] animated-text">
        TA'LIM BOSQICHLARI
      </h1>
      <div class="iconsAnim flex items-center justify-center flex-col">
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
          <div class="line1 text-[#E0E0E0] text-[30px] mt-[20px]">
            - - - - - -
          </div>
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/triogonometry.svg" alt="#" />
            <img
              src="/src/assets/icons/down-arrow.svg"
              class="downArrow bg-[#E0E0E0] p-[8px] rounded-[50px]"
              alt="#"
            />
            <p class="text-[#1B1B35] text-[18px]">Amaliy kurs</p>
          </div>
        </div>
        <div
          class="line2 text-[#E0E0E0] text-[30px] flex items-end justify-end mt-[30px] ml-[230px] rotate-90"
        >
          - - - -
        </div>
        <div class="level1 flex items-center justify-center mt-[35px]">
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/nurce.svg" alt="#">
            <img src="/src/assets/icons/left-arrow.svg" class="leftArrow bg-[#E0E0E0] p-[8px] rounded-[50px]" alt="#">
            <p class="text-[#1B1B35] text-[18px]">YHXX imtihoni</p>
          </div>
          <div class="line3 text-[#E0E0E0] text-[30px] mt-[20px]">- - - - - -</div>
          <div class="lamp flex items-center justify-center flex-col gap-[5px]">
            <img src="/src/assets/icons/done_job.svg" alt="#">
            <img src="/src/assets/icons/check-circle.svg" class="done bg-[#E0E0E0] p-[8px] rounded-[50px]" alt="#">
            <p class="text-[#1B1B35] text-[18px]">Ichki imtihon</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.animated-text {
  animation: colorChange 2s;
  background: linear-gradient(to right, #E0E0E0, #1B1B35);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  display: inline-block;
  animation-fill-mode: forwards;
}

@keyframes colorChange {
  0% {
    color: #E0E0E0;
  }
  100% {
    color: #1B1B35;
  }
}

.line1{
  animation: colorChangeLine 2s ;
  background: linear-gradient(to right, #E0E0E0, #407BFF);
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
    color: #E0E0E0;
  }
  100% {
    background-position: 100% 0%;
    color: #407BFF;
  }
}

.downArrow{
  animation: colorChangeDown 2s ;
  animation-fill-mode: forwards;
  animation-delay: 1s;
}

@keyframes colorChangeDown {
  0% {
    background: #E0E0E0;
  }
  100% {
    background: #407BFF;
  }
}

.line2{
  animation: colorChangeLine2 2s ;
  color: linear-gradient(to right, #E0E0E0, #407BFF);
  animation-fill-mode: forwards;
  animation-delay: 2s;
}

@keyframes colorChangeLine2 {
  0% {

    color: #E0E0E0;
  }
  100% {

    color: #407BFF;
  }
}

.done{
  animation: colorChangeDown 2s ;
  animation-fill-mode: forwards;
  animation-delay: 3s;
}

@keyframes colorChangeDown {
  0% {
    background: #E0E0E0;
  }
  100% {
    background: #407BFF;
  }
}

.line3{
  animation: colorChangeLine3 2s ;
  color: linear-gradient(to right, #E0E0E0, #407BFF);
  animation-fill-mode: forwards;
  animation-delay: 4s;
}

@keyframes colorChangeLine3 {
  0% {

    color: #E0E0E0;
  }
  100% {

    color: #407BFF;
  }
}

.leftArrow{
  animation: colorChangeDown 2s ;
  animation-fill-mode: forwards;
  animation-delay: 5s;
}
</style>

<!-- #407BFF blue #E0E0E0 default -->

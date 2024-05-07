<template>
  <div id="home">
    <section
      class="flex items-center justify-between max-w-[1388px] m-auto pt-[35px] px-3"
    >
      <div class="flex flex-col items-center">
        <p class="text-blue text-[50px] font-semibold leading-[75px] uppercase">
          Creatic
        </p>
        <p class="text-white text-sm font-normal leading-5 tracking-[2px]">
          CREATIVE AGENCY
        </p>
      </div>
      <div
        class="text-white font-normal text-[21px] leading-8 flex w-full justify-between max-w-[939px] pb-[19px] max-[1450px]:hidden"
      >
        <a href="#home">Home</a>
        <a href="#about">About us</a>
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#pages">Pages</a>
        <a href="#contact">Contact Us</a>
        <img :src="search" alt="search" />
      </div>
      <div @click="click_modal" class="cursor-pointer">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="30"
          height="30"
          fill="currentColor"
          class="bi bi-list text-white max-[1450px]:block hidden"
          viewBox="0 0 16 16"
        >
          <path
            fill-rule="evenodd"
            d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"
          />
        </svg>
      </div>
      <div
        v-if="show_modal"
        class="text-black fixed right-0 left-0 top-0 w-full h-[100vh] bg-white font-normal text-[21px] leading-8 justify-between pb-[19px] min-[1450px]:hidden"
      >
        <span
          @click="show_modal = false"
          class="flex justify-end absolute top-[65px] right-[20px] cursor-pointer"
          >X</span
        >
        <div
          class="flex flex-col items-center relative top-2/4 transform translate-y-[-50%] gap-[14px]"
        >
          <a @click="show_modal = false" href="#home">Home</a>
          <a @click="show_modal = false" href="#about">About us</a>
          <a @click="show_modal = false" href="#services">Services</a>
          <a @click="show_modal = false" href="#portfolio">Portfolio</a>
          <a @click="show_modal = false" href="#pages">Pages</a>
          <a @click="show_modal = false" href="#contact">Contact Us</a>
        </div>
      </div>
    </section>
    <section>
      <div class="asd mt-[50px] pt-[135px]">
        <div class="max-w-[1388px] m-auto px-3">
          <div class="flex flex-col gap-[43px] max-w-[819px] w-full">
            <p
              class="text-blue text-[21px] font-medium leading-8 tracking-[2px]"
            >
              Welcome to creatic
            </p>
            <div>
              <h1 class="text-white text-[4vw] font-bold leading-[111.49%]">
                WE ARE <span class="text-blue"> CREATIVE</span> DESIGN AGENCY
              </h1>
              <div
                class="border-[3px] border-solid border-blue w-[144px] mt-[41px]"
              ></div>
              <p
                class="text-white text-[21px] font-light leading-[32px] pt-[44px]"
              >
                Lorem ipsumNeque porro quisquam est qui dolorem ipsum quia dolor
                sit amet, consectetur, adipisci velit Neque porro elit Neque
                porro quis ipsum
              </p>
            </div>
            <button
              class="text-white hover:bg-blue hover:text-black hover:border-white font-normal w-fit text-[17px] leading-[26px] tracking-[2px] border-[3px] border-solid rounded-[2px] border-blue px-[16px] py-[10px]"
            >
              GET IN TOUCH
            </button>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import search from "@/assets/images/search.svg";
import woman from "@/assets/images/woman.png";
import { ref } from "vue";
const show_modal = ref(false);
const click_modal = () => {
  show_modal.value = !show_modal.value;
};
</script>
<style scoped>
.asd {
  background: linear-gradient(
      -82.82deg,
      rgba(109, 149, 252, 0.67) -53.756%,
      rgba(109, 149, 252, 0) 29.836%
    ),
    url("../assets/images/woman.png");
  height: 787px;
  width: 100%;
  background-repeat: no-repeat;
  background-position: right;
  background-size: contain;
}
</style>

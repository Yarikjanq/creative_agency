<template>
  <section id="contact" class="flex max-[1070px]:flex-col">
    <div class="flex-1 max-[1070px]:pb-10">
      <div
        class="max-w-[483px] block m-auto mt-[172px] mr-[110px] max-[1070px]:m-auto px-3"
      >
        <p class="text-[48px] font-bold leading-[72px] text-white">
          GET IN <span class="text-blue">TOUCH</span>
        </p>
        <div class="border-[3px] border-white w-[100px] mt-[30px]"></div>
        <p class="text-[21px] font-light leading-[166.5%] text-white py-[30px]">
          Lorem ipsum Neque porro quisquam est qui do lorem ipsum quia dolor sit
          amet, Neque porro elit NeDque porro
        </p>
        <div class="flex flex-col gap-[39px]">
          <div class="flex gap-[33px] items-center">
            <div><img :src="adress" alt="" /></div>
            <p class="text-white">
              Office Address <br />
              <span class="text-blue"
                >98, Arca St, PR City, 33414 , Indonesia</span
              >
            </p>
          </div>
          <div class="flex gap-[33px] items-center">
            <div><img :src="phone" alt="" /></div>
            <p class="text-white">
              Call Us <br />
              <span class="text-blue">(+BK) 123 456 7891</span>
            </p>
          </div>
          <div class="flex gap-[33px] items-center">
            <div><img :src="mail" alt="" /></div>
            <p class="text-white">
              Mail Us <br />
              <span class="text-blue">info@creaticagency.com</span>
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="flex-1 background">
      <div
        class="mail p-[30px] max-w-[426px] w-full max-[1070px]:max-w-full ml-[37px] mt-[134px] max-[1070px]:m-auto flex flex-col gap-[22px]"
      >
        <div>
          <p class="text-white text-[17px] font-normal">YOUR NAME</p>
          <input
            v-model="your_name"
            class="border-[1px] outline-0 h-[50px] w-full border-solid border-white bg-transparent text-white px-5"
            type="text"
          />
          <div v-if="show_error_name" class="text-red-600">asdadad</div>
        </div>
        <div>
          <p class="text-white text-[17px] font-normal">YOUR EMAIL</p>
          <input
            v-model="your_email"
            class="border-[1px] outline-0 h-[50px] w-full border-solid border-white bg-transparent text-white px-5"
            type="email"
          />
          <div v-if="show_error_email" class="text-red-600">EMAIL SUKA</div>
        </div>
        <div>
          <p class="text-white text-[17px] font-normal">YOUR MESSAGE</p>
          <textarea
            class="bg-transparent outline-0 w-full border-[1px] border-solid border-white h-[178px] text-white px-5 py-5"
          ></textarea>
        </div>
        <button
          @click="send_msg"
          class="text-[#111728] hover:bg-black hover:text-blue hover:border-white bg-[#6D95FC] text-[17px] font-medium leading-[26px] px-[16px] py-[10px] block m-auto mt-[32px]"
        >
          SEND MESSAGE
        </button>
      </div>
    </div>
  </section>
  <!-- CREATIC -->
  <section>
    <div class="pt-[133px]">
      <p
        class="text-blue text-[55px] font-semibold leading-[83px] text-center flex flex-col"
      >
        CREATIC <br /><span
          class="text-white text-[14px] font-normal leading-[21px]"
          >CREATIVE AGENCY</span
        >
      </p>
      <div
        class="w-[100px] border-[2px] border-solid border-white m-auto mt-[20px]"
      ></div>
      <ul
        class="flex gap-[21px] justify-center max-[572px]:flex-col max-[572px]:items-center"
      >
        <li class="text-blue text-[21px] font-medium leading-8">Categories</li>
        <li class="text-blue text-[21px] font-medium leading-8">About</li>
        <li class="text-blue text-[21px] font-medium leading-8">Services</li>
        <li class="text-blue text-[21px] font-medium leading-8">Portfolio</li>
        <li class="text-blue text-[21px] font-medium leading-8">Pages</li>
        <li class="text-blue text-[21px] font-medium leading-8">Support</li>
      </ul>
      <p
        class="text-[21px] font-light leading-[166.5%] text-white text-center pt-[20px]"
      >
        Lorem ipsum Neque porro quisquam est qui do lorem ipsum <br />
        quia dolor sit amet, Neque porro elit NeDque
      </p>
      <ul class="flex justify-center gap-[26px] pt-[20px]">
        <img :src="facebook" alt="" />
        <img :src="insta" alt="" />
        <img :src="viber" alt="" />
        <img :src="ina" alt="" />
        <img :src="D" alt="" />
        <img :src="twitter" alt="" />
      </ul>
    </div>
  </section>
  <div class="footer h-[253px]"></div>
</template>
<script setup lang="ts">
import adress from "@/assets/images/adress.svg";
import phone from "@/assets/images/phone.svg";
import mail from "@/assets/images/mail.svg";
import facebook from "@/assets/images/facebook.svg";
import insta from "@/assets/images/insta.svg";
import ina from "@/assets/images/in.svg";
import D from "@/assets/images/D.svg";
import twitter from "@/assets/images/twitter.svg";
import viber from "@/assets/images/viber.svg";
import { ref } from "vue";

const your_name = ref("");
const your_email = ref("");
const show_error_name = ref(false);
const show_error_email = ref(false);
const send_msg = () => {
  if (your_name.value === "") {
    show_error_name.value = true;
  } else {
    show_error_name.value = false;
  }
  if (your_email.value === "") {
    show_error_email.value = true;
  } else {
    show_error_email.value = false;
  }
  if (your_name.value.length > 4) {
    console.error("HUI");
  } else {
    console.log({ name: your_name.value, email: your_email.value });
  }
};
</script>

<style>
.background {
  background: linear-gradient(
    192.46deg,
    rgba(109, 149, 252, 0.24) 11.025%,
    rgba(21, 21, 21, 0) 90.87%
  );
}
.mail {
  border-radius: 34px;

  background: linear-gradient(
    180deg,
    rgb(18, 25, 43),
    rgba(18, 25, 43, 0) 109.076%
  );
}
.footer {
  filter: blur(500px);
  background: rgb(109, 149, 252);
}
</style>

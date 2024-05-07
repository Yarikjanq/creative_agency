<template>
  <section class="flex justify-between">
    <div class="max-[1484px]:w-full">
      <img class="max-[1484px]:w-full" :src="image" alt="" />
    </div>
    <div class="pt-[68px] max-[1484px]:hidden">
      <div>
        <p
          class="text-[2.71vw] font-bold leading-[109.5%] text-white text-center pb-[10px]"
        >
          WHAT <span class="text-blue">OUR</span><br />
          CLEINTS SAY?
        </p>
        <p class="border-b-[3px] border-solid border-blue w-[218px] m-auto"></p>
        <p
          class="text-[21px] font-normal leading-8 text-white text-center pt-[13px]"
        >
          TESTIMONIALS
        </p>
      </div>
      <div>
        <div class="w-fit m-auto">
          <div class="client p-[38px_57px_34px_67px]">
            <p
              class="text-[21px] font-light leading-[166.5%] text-white max-w-[424px] pb-[40px]"
            >
              Lorem ipsum Neque porro quisquam est qui do lorem ipsum quia dolor
              sit amet, Neque porro elit
            </p>
            <div class="flex items-center gap-4 px-[13px]">
              <img :src="face" alt="face" />
              <div class="flex items-start justify-between w-full">
                <p class="text-white text-[21px] font-bold leading-[166.5%]">
                  Carol Chaves <br />
                  <span
                    class="text-[14px] font-light leading-[166.5%] text-blue"
                    >@caroles.gmail.com</span
                  >
                </p>
                <div class="flex gap-[2px]">
                  <img class="pt-[10px]" :src="comma" alt="comma" />
                  <img class="pt-[10px]" :src="comma" alt="comma" />
                </div>
              </div>
            </div>
          </div>
          <button
            class="text-white block m-auto font-normal w-fit text-[17px] leading-[26px] mt-[77px] tracking-[2px] border-[3px] border-solid rounded-[2px] border-blue px-[16px] py-[10px]"
          >
            VIEW ALL TESTIMONIALS
          </button>
        </div>
      </div>
    </div>
    <div class="max-[1484px]:w-full">
      <img class="max-[1484px]:w-full" :src="image2" alt="" />
    </div>
  </section>
</template>
<script setup>
import face from "@/assets/images/face.png";
import comma from "@/assets/images/comma.svg";
import image from "@/assets/images/Image.png";
import image2 from "@/assets/images/Image2.png";
</script>
<style>
.client {
  border-radius: 38px;

  background: linear-gradient(
    178.44deg,
    rgba(17, 24, 42, 0.7) 19.668%,
    rgba(17, 24, 42, 0) 121.51%
  );
}
</style>

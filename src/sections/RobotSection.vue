<template>
  <!-- About us -->
  <div id="about" class="flex max-[980px]:flex-col px-3">
    <div class="max-w-[863px]">
      <img class="w-full h-full" :src="robot" alt="robot" />
    </div>
    <div class="max-w-[1388px] m-auto">
      <div class="flex flex-col gap-[26px] max-w-[708px] w-full">
        <p class="text-blue text-[21px] font-medium leading-8 tracking-[2px]">
          ABOUT US
        </p>

        <h1 class="text-white text-[48px] font-bold leading-[111.49%]">
          We Bring <span class="text-blue"> Creative</span> ideas to life.
        </h1>
        <div class="border-[3px] border-solid border-blue w-[144px]"></div>

        <p class="text-[17px] font-normal leading-26px text-blue">
          We love Creating
        </p>
        <p class="text-white text-[21px] font-light leading-[32px]">
          Lorem ipsumNeque porro quisquam est qui do lorem ipsum quia dolor sit
          amet, Neque porro elit NeDque porro Lorem ipsum Neque porro<br /><br />
          Neque porro Neque porro quisquam est qui do lorem ipsum quia dolor sit
          amet, Lorem ipsum Neque quis ipsum
        </p>

        <button
          class="text-white hover:bg-blue hover:text-black hover:border-white font-normal w-fit text-[17px] leading-[26px] tracking-[2px] border-[3px] border-solid rounded-[2px] border-blue px-[16px] py-[10px]"
        >
          READ MORE
        </button>
      </div>
    </div>
  </div>
  <!-- Our Services -->
  <section>
    <div
      id="services"
      class="asd mt-[50px] pt-[135px] flex items-center justify-center gap-[91px] w-fit m-auto max-[1322px]:flex-col"
    >
      <div class="max-w-[1388px] m-auto px-3">
        <div class="flex flex-col gap-[32px] max-w-[589px] w-full">
          <p class="text-blue text-[21px] font-medium leading-8 tracking-[2px]">
            OUR SERVICES
          </p>
          <div>
            <h1 class="text-white text-[48px] font-bold leading-[111.49%]">
              Experience The Power of <span class="text-blue"> Innovation</span>
            </h1>
            <div
              class="border-[3px] border-solid border-white w-[144px] mt-[41px]"
            ></div>
            <p
              class="text-white text-[21px] font-light leading-[32px] pt-[44px]"
            >
              Lorem ipsum Neque porro quisquam est qui do lorem ipsum quia dolor
              sit amet, Neque porro elit NeDque porro Neque porro quisquam est
              qui do lorem ipsum quia dolor sit amets ipsum
            </p>
          </div>
          <button
            class="text-white hover:bg-blue hover:text-black hover:border-white font-normal w-fit text-[17px] leading-[26px] tracking-[2px] border-[3px] border-solid rounded-[2px] border-blue px-[16px] py-[10px]"
          >
            VIEW ALL
          </button>
        </div>
      </div>
      <div
        class="grid grid-rows-2 grid-flow-col max-[636px]:grid-flow-row w-max max-[636px]:gap-14"
      >
        <div class="max-w-[300px] p-[30px] flex items-center flex-col video">
          <div class="">
            <img :src="video" alt="video" />
          </div>
          <p
            class="text-[21px] font-semibold leading-8 text-blue flex flex-col items-center"
          >
            VIDEO MARKETING
            <span
              class="text-[17px] text-white font-light leading-[122.5%] text-center tracking-[0.833px]"
            >
              Lorem ipsum Neque do porro quisquam est qui do quam
            </span>
          </p>
        </div>
        <div class="max-w-[300px] p-[30px] flex items-center flex-col graphic">
          <div class="">
            <img :src="video" alt="video" />
          </div>
          <p
            class="text-[21px] font-semibold leading-8 text-blue flex flex-col items-center"
          >
            VIDEO MARKETING
            <span
              class="text-[17px] text-white font-light leading-[122.5%] text-center tracking-[0.833px]"
            >
              Lorem ipsum Neque do porro quisquam est qui do quam
            </span>
          </p>
        </div>
        <div class="max-w-[300px] p-[30px] flex items-center flex-col video-2">
          <div class="">
            <img :src="video" alt="video" />
          </div>
          <p
            class="text-[21px] font-semibold leading-8 text-blue flex flex-col items-center"
          >
            VIDEO MARKETING
            <span
              class="text-[17px] text-white font-light leading-[122.5%] text-center tracking-[0.833px]"
            >
              Lorem ipsum Neque do porro quisquam est qui do quam
            </span>
          </p>
        </div>
        <div class="max-w-[300px] p-[30px] flex items-center flex-col website">
          <div class="">
            <img :src="video" alt="video" />
          </div>
          <p
            class="text-[21px] font-semibold leading-8 text-blue flex flex-col items-center"
          >
            VIDEO MARKETING
            <span
              class="text-[17px] text-white font-light leading-[122.5%] text-center tracking-[0.833px]"
            >
              Lorem ipsum Neque do porro quisquam est qui do quam
            </span>
          </p>
        </div>
      </div>
    </div>
    <div class="oa mt-[154px]">
      <div
        class="flex max-w-[1351px] justify-between m-auto pt-[83px] pb-[65px] max-[765px]:flex-col max-[765px]:items-center max-[765px]:gap-[50px]"
      >
        <div class="">
          <div
            class="flex flex-col items-center justify-center max-w-[189px] w-full"
          >
            <div>
              <img class="w-full h-full" :src="team" alt="" />
            </div>
            <p class="text-[64px] font-bold text-white leading-none">50+</p>
            <p class="text-[21px] font-normal leading-[122.5%] text-blue">
              Team members
            </p>
          </div>
        </div>

        <div class="">
          <div
            class="flex flex-col items-center justify-center max-w-[189px] w-full"
          >
            <div class="h-[91px]">
              <img class="w-full h-full" :src="project" alt="" />
            </div>
            <p class="text-[64px] font-bold text-white leading-none">200+</p>
            <p class="text-[21px] font-normal leading-[122.5%] text-blue">
              Project done
            </p>
          </div>
        </div>
        <div class="">
          <div
            class="flex flex-col items-center justify-center max-w-[189px] w-full"
          >
            <div>
              <img class="w-full h-full" :src="customers" alt="" />
            </div>
            <p class="text-[64px] font-bold text-white leading-none">500+</p>
            <p class="text-[21px] font-normal leading-[122.5%] text-blue">
              Happy customers
            </p>
          </div>
        </div>
        <div class="">
          <div
            class="flex flex-col items-center justify-center max-w-[189px] w-full"
          >
            <div>
              <img class="w-full h-full" :src="award" alt="" />
            </div>
            <p class="text-[64px] font-bold text-white leading-none">75+</p>
            <p class="text-[21px] font-normal leading-[122.5%] text-blue">
              Award Winning
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import robot from "@/assets/images/robot.png";
import video from "@/assets/images/video.svg";
import team from "@/assets/images/team.svg";
import project from "@/assets/images/project.svg";
import customers from "@/assets/images/customers.svg";
import award from "@/assets/images/award.svg";
</script>
<style scoped>
.video {
  background: linear-gradient(
    90deg,
    rgba(109, 149, 252, 0.35) -346.667%,
    rgba(21, 21, 21, 0.31) 74.833%
  );
}
.graphic {
  background: linear-gradient(
    2.22deg,
    rgba(109, 149, 252, 0.55) -180.084%,
    rgba(109, 149, 252, 0) 67.518%
  );
}
.website {
  background: linear-gradient(
    to left,
    rgba(109, 149, 252, 0.55) -217.333%,
    rgba(109, 149, 252, 0) 66.643%
  );
}
.video-2 {
  background: linear-gradient(
    180deg,
    rgba(109, 149, 252, 0.55) -217.333%,
    rgba(109, 149, 252, 0) 66.643%
  );
}
.oa {
  background: linear-gradient(
    270deg,
    rgb(109, 149, 252) -127.552%,
    rgba(21, 21, 21, 0.35) 77.969%
  );
}
</style>

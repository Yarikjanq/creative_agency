<template>
  <div id="pages" class="pt-[110px]">
    <div class="flex items-center justify-center flex-col gap-[50px] pb-[50px]">
      <p class="text-white text-[48px] font-bold leading-[136.5%] text-center">
        ENJOY OUR <span class="text-blue">LATEST <br /></span> PROJECTS
      </p>
      <div class="flex gap-[14.5px] items-center">
        <p class="border-[3px] border-solid border-white w-[100px]"></p>
        <p class="text-blue text-[21px] font-medium leading-8">OUR WORK</p>
        <p class="border-[3px] border-solid border-white w-[100px]"></p>
      </div>
    </div>
    <Carousel :itemsToShow="3" :wrapAround="true" :transition="500">
      <Slide v-for="slide in images" :key="slide.url">
        <img :src="slide.url" class="carousel__item bg-white w-full h-full" />
      </Slide>
      <template #addons>
        <Navigation />
        <Pagination class="pagination" />
      </template>
    </Carousel>
  </div>
  <section id="portfolio" class="flex pt-[121px] max-[765px]:flex-col">
    <div class="flex-1 pb-[250px] max-[765px]:pb-0 px-3">
      <div class="max-w-[770px] m-auto mr-0 w-fit pt-[60px]">
        <p
          class="text-[21px] font-normal leading-8 text-white border-b-[3px] border-solid border-blue w-[110px] flex items-center justify-center"
        >
          WHY US?
        </p>
        <h1
          class="text-white text-[55px] font-bold leading-[110%] pt-[25px] pb-[55px]"
        >
          25 YEAR OF <span class="text-blue"> EXPERIENCE <br /></span>AS A
          CREATIVE AGENCY
        </h1>
        <button
          class="text-white hover:bg-blue hover:text-black hover:border-white font-normal w-fit text-[17px] leading-[26px] tracking-[2px] border-[3px] border-solid rounded-[2px] border-blue px-[16px] py-[10px]"
        >
          READ MORE
        </button>
      </div>
    </div>
    <div
      class="gradient flex-1 text-white text-[21px] font-light leading-[166.5%] flex flex-col gap-[40px]"
    >
      <div
        class="max-w-[485px] pt-[113px] max-[764px]:px-3 pl-[60px] flex flex-col gap-[32px]"
      >
        <p>
          Lorem ipsum Neque porro quisquam est qui do lorem ipsum quia dolor sit
          amet, Neque porro elit NeDque porro Lorem ipsum
        </p>
        <ul>
          <li class="flex gap-[11px]">
            <img :src="correct" alt="" />
            <p class="text-[21px] font-light leading-[166.5%] text-white">
              Happy Customer
            </p>
          </li>
          <li class="flex gap-[11px]">
            <img :src="correct" alt="" />
            <p class="text-[21px] font-light leading-[166.5%] text-white">
              Experienced Team
            </p>
          </li>
          <li class="flex gap-[11px]">
            <img :src="correct" alt="" />
            <p class="text-[21px] font-light leading-[166.5%] text-white">
              Modern Technology
            </p>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
import team from "@/assets/images/team.svg";
import project from "@/assets/images/project.png";
import project2 from "@/assets/images/project2.png";
import project3 from "@/assets/images/project3.png";
import correct from "@/assets/images/correct.svg";
import { Carousel, Pagination, Slide } from "vue3-carousel";
import "vue3-carousel/dist/carousel.css";

const images = ref([{ url: project2 }, { url: project3 }, { url: project }]);
</script>
<style>
.gradient {
  background: linear-gradient(
    to top,
    rgba(109, 149, 252, 0.24) 11.025%,
    rgba(21, 21, 21, 0) 90.87%
  );
}
.carousel__slide {
  padding: 5px;
}

.carousel__viewport {
  perspective: 2000px;
}

.carousel__track {
  transform-style: preserve-3d;
}

.carousel__slide--sliding {
  transition: 0.5s;
}

.carousel__slide {
  opacity: 0.9;
  transform: rotateY(-20deg) scale(0.9);
}

.carousel__slide--active ~ .carousel__slide {
  transform: rotateY(20deg) scale(0.9);
}

.carousel__slide--prev {
  opacity: 1;
  transform: rotateY(-10deg) scale(0.95);
}

.carousel__slide--next {
  opacity: 1;
  transform: rotateY(10deg) scale(0.95);
}

.carousel__slide--active {
  opacity: 1;
  transform: rotateY(0) scale(1.1);
}
.pagination .carousel__pagination-item .carousel__pagination-button::after {
  background: white;
}
.pagination
  .carousel__pagination-item
  .carousel__pagination-button--active::after {
}
.pagination .carousel__pagination-item .carousel__pagination-button--active {
  padding: 5px;
  border: 1px solid blue !important;
}
.pagination .carousel__pagination-item .carousel__pagination-button {
  padding: 5px;
  border: 1px solid;
}
</style>

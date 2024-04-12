<script>
import {Swiper, SwiperSlide} from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/free-mode';
import 'swiper/css/pagination';

import {FreeMode, Pagination} from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      slides: [
        { color: '#FFBE21' },
        { color: '#4756DF' },
        { color: '#3EC1F3' },
        { color: '#FFBE21' },
        { color: '#4756DF' },
        { color: '#3EC1F3' },
        { color: '#FFBE21' },
        { color: '#4756DF' },
        { color: '#3EC1F3' },
        { color: '#FFBE21' },
        { color: '#4756DF' },
        { color: '#3EC1F3' },
      ],
      modules: [FreeMode, Pagination],
    };
  },
};
</script>

<template>
  <div class="wrapper d-flex flex-column justify-space-between" style="height: 800px">
    <div class="d-flex flex-column align-center">
      <div style="margin-top: 121px; width: 920px;" class="text-center">
      <span class="font-weight-bold" style="font-size: 96px; color:#292830; line-height: 96px">
        We have millions of best wishers
      </span>
      </div>
    </div>
      <div style="margin-bottom: 121px">
        <swiper
          style="--swiper-pagination-color: #292830;
          --swiper-pagination-bullet-inactive-color: #FFFFFF;
          --swiper-pagination-bullet-inactive-opacity: 0.1;
          --swiper-pagination-bullet-size: 12px;"
          :slidesPerView="5"
          :spaceBetween="30"
          :pagination="{
        clickable:true,
      }"
          :modules="modules"
          class="mySwiper"
        >
          <swiper-slide v-for="slide in slides" style="width: 350px !important;height: 316px !important;">
            <v-card class="d-flex flex-column pl-7 pr-7 justify-space-evenly" height="240px"
                    :style="`border-top: 10px solid ${slide.color} `">
              <div class="mb-2" style="font-size: 18px; color:#000000; line-height: 29px">
          <span>
            Eleifend fames amet, fames enim. Ullamcorper pellentesque ac volutpat nibh aliquet et, ut netus. Vel, fringilla sit eros pretium felis massa mauris, aliquam congue.
          </span>
              </div>
              <div class="d-flex align-center">
                <div class="mr-3">
                  <v-img src="/Madam.png" height="30" width="30"></v-img>
                </div>
                <div>
            <span class="font-weight-bold" style="font-size: 16px; color:#292830; line-height: 25px">
            Cameron Williamson,
          </span>
                  <span style="font-size: 16px; color:#BDBDBD; line-height: 25px">
             CEO
          </span>
                </div>
              </div>
            </v-card>
          </swiper-slide>
        </swiper>
      </div>
  </div>
</template>

<style scoped>
.swiper-pagination-bullet {
  border: 2px solid red;
}
</style>

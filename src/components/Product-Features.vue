<script setup>
import { ref } from 'vue';

const hoveredCardIndex = ref(-1);

const handleMouseEnter = (index) => {
  hoveredCardIndex.value = index;
};

const handleMouseLeave = () => {
  hoveredCardIndex.value = -1;
};

const cardStyle = (index) => ({
  boxShadow: hoveredCardIndex.value === index ? '0 0 50px 0 #0000000A' : 'none',
  cursor: 'pointer',
});

const isHovered = (index) => hoveredCardIndex.value === index;
</script>


<template>
<div class="wrapper d-flex align-center" style="height: 900px">
  <div class="container ">

    <div class="d-flex align-center" style="max-height: 192px; margin-bottom: 80px;">

      <div style="height: 192px;">
        <span class="font-weight-bold" style="font-size: 96px; line-height: 96px; color:#292830; height: 192px;">
          The Product we work with.
        </span>
      </div>

      <div style="max-width: 350px; height: 156px;">
        <span style="color:#BDBDBD; font-size: 24px; line-height: 38px;">
          Tellus lacus morbi sagittis lacus in. Amet nisl at mauris enim aumsan nisi, tincidunt vel. Enim ipsum, at quis ullamcorper eget ut.
        </span>
      </div>

    </div>

    <div class="d-flex align-center justify-space-between">
      <div class="d-flex align-center">
        <v-card
          @mouseenter="handleMouseEnter(1)"
          @mouseleave="handleMouseLeave(1)"
          :style="cardStyle(1)"
          variant="flat"
          class="d-flex flex-column align-center justify-center"
          width="350"
          height="350">
          <div class="mb-6 rounded-circle d-flex justify-center align-center" style="background-color:#FFBD740D; width: 64px; height: 64px;">
            <v-img  src="/Notebook.png" style="width: 24px; height: 16px"></v-img>
          </div>
          <div class="mb-3 d-flex justify-center align-center">
            <span style="font-size: 30px; line-height: 30px;" class="font-weight-medium">
              Cross platform
            </span>
          </div>
          <div class="text-center" style="width: 220px; font-size: 14px; line-height: 22px; color: #BDBDBD; margin-bottom: 24px">
            <span>
              Elit esse cillum dolore eu fugiat nulla <br> pariatur
            </span>
          </div>
          <div v-if="isHovered(1)" class="overlay" style="width: 16px; height: 8px;">
            <v-img src="/big-black-arrow-right.png"></v-img>
          </div>
        </v-card>
      </div>
      <div class="d-flex align-center">
        <v-card
          @mouseenter="handleMouseEnter(2)"
          @mouseleave="handleMouseLeave(2)"
          :style="cardStyle(2)"
          class="d-flex flex-column align-center justify-center"
          width="350"
          height="350"
        >
          <div class="mb-6 rounded-circle d-flex justify-center align-center" style="background-color:#E2598B0D; width: 64px; height: 64px;">
            <v-img  src="/Cloud.png" style="width: 24px; height: 16px"></v-img>
          </div>
          <div class="mb-3 d-flex justify-center align-center">
            <span style="font-size: 30px; line-height: 30px;" class="font-weight-medium">
              Cloud server
            </span>
          </div>
          <div style="width: 220px; font-size: 14px; line-height: 22px; color: #BDBDBD; margin-bottom: 24px">
            <span>
              Elit esse cillum dolore eu fugiat nulla
            </span>
            <span class="d-flex justify-center align-center">
              pariatur
            </span>
          </div>
          <div v-if="isHovered(2)" class="overlay" style="width: 16px; height: 8px;">
            <v-img src="/big-black-arrow-right.png"></v-img>
          </div>
        </v-card>
      </div>
      <div class="d-flex align-center">
        <v-card
          @mouseenter="handleMouseEnter(3)"
          @mouseleave="handleMouseLeave(3)"
          :style="cardStyle(3)"
          variant="flat"
          class="d-flex flex-column align-center justify-center"
          width="350"
          height="350">
          <div class="mb-6 rounded-circle d-flex justify-center align-center" style="background-color:#4D12EE0D; width: 64px; height: 64px;">
            <v-img  src="/Battery.png" style="width: 24px; height: 16px"></v-img>
          </div>
          <div class="mb-3 d-flex justify-center align-center">
            <span style="font-size: 30px; line-height: 30px;" class="font-weight-medium">
              Pure Java
            </span>
          </div>
          <div style="width: 220px; font-size: 14px; line-height: 22px; color: #BDBDBD; margin-bottom: 24px">
            <span>
              Elit esse cillum dolore eu fugiat nulla
            </span>
            <span class="d-flex justify-center align-center">
              pariatur
            </span>
          </div>
          <div v-if="isHovered(3)" class="overlay" style="width: 16px; height: 8px;">
            <v-img src="/big-black-arrow-right.png"></v-img>
          </div>
        </v-card>
      </div>
    </div>

  </div>
</div>
</template>

<style scoped>

</style>

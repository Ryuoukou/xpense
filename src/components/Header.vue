<script setup>
import { ref } from 'vue'

const scrollToTop = ref(() => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth'
  });
});
</script>

<template>
        <div style="background-color:#FFFFFF; position: fixed;z-index: 999" class="pt-15 wrapper">
          <div class="d-flex justify-space-between align-center pb-2 container">
            <div class="d-flex justify-space-between align-center">
              <v-img src="/X.png" align-start width="40" height="40" class="mr-3 cursor-pointer" @click="scrollToTop"></v-img>
              <span class="font-weight-medium" style="font-size: 23px">pense</span>
            </div>
            <div class="nav d-flex justify-space-between align-center" style="font-size: 18px">
              <span class="mr-10 cursor-pointer">Features</span>
              <span class="mr-10 cursor-pointer">About us</span>
              <span class="mr-10 cursor-pointer">Pricing</span>
              <span class="mr-10 cursor-pointer">Feedback</span>
            </div>
            <div class="d-flex justify-center align-center">
              <v-btn color="#FF7235" variant="outlined" class="rounded-lg font-weight-regular text-none">Request a demo</v-btn>
            </div>
          </div>
        </div>
</template>

<style scoped>
.nav span {
  height: 17px;
}
</style>

<script setup>
import { ref } from "vue";
import axios from "axios";

const email = ref('');
const isEmailValid = ref(false)

const emailRule = [
  (value) => !!value || 'Email is required',
  (value) => {
    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    const isValid = emailRegex.test(value);
    isEmailValid.value = isValid;
    return isValid || 'Invalid email';
  }
];

const subscribeAndClear = async () => {
  if (!isEmailValid.value) {
    return;
  }

  try {
    const response = await axios.post("https://d45294201c0fb43f.mokky.dev/subscribe", {
      email: email.value,
    });
    console.log(response.data);
    email.value = '';
  } catch (error) {
    console.log(error)
  }
};
</script>

<template>
<div class="wrapper" style="height: 530px;">
  <div class="d-flex justify-space-between mb-10 container">
    <div class="d-flex">
      <v-img src="/X.png" align-start width="40" height="40" class="mr-3"></v-img>
      <span class="font-weight-medium" style="font-size: 23px">pense</span>
    </div>

    <div class="d-flex flex-column">
      <div style="margin-bottom: 24px; font-size: 24px; line-height: 38px; font-weight: 500; color: #292830; text-transform: uppercase">
        <span>
          Links
        </span>
      </div>
      <div class="d-flex flex-column" style="font-size: 18px; line-height: 29px; font-weight: 500; color: #292830">
        <span class="mb-2">
          Home
        </span>
        <span class="mb-2">
          About us
        </span>
        <span class="mb-2">
          Careers
        </span>
        <span class="mb-2">
          Pricing
        </span>
        <span class="mb-2">
          Features
        </span>
        <span>
          Blog
        </span>
      </div>
    </div>

    <div class="d-flex flex-column">
      <div style="margin-bottom: 24px; font-size: 24px; line-height: 38px; font-weight: 500; color: #292830; text-transform: uppercase">
        <span>
          Legal
        </span>
      </div>
      <div class="d-flex flex-column" style="font-size: 18px; line-height: 29px; font-weight: 500; color: #292830">
        <span class="mb-2">
          Terms of use
        </span>
        <span class="mb-2">
          Terms of conditions
        </span>
        <span class="mb-2">
          Privecy policy
        </span>
        <span>
          Cookie policy
        </span>
      </div>
    </div>

    <div class="d-flex flex-column">
      <div style="margin-bottom: 24px; font-size: 24px; line-height: 38px; font-weight: 500; color: #292830; text-transform: uppercase">
        <span>
          Newsletter
        </span>
      </div>
      <div class="d-flex flex-column">
        <span style="margin-bottom: 18px; font-size: 20px; line-height: 32px; font-weight: 400; color: #BDBDBD">
          Over 25000 people have subscribed
        </span>
        <v-text-field
          v-model="email"
          :rules="emailRule"
          style="width: 349px; height: 62px; margin-bottom: 16px;"
          color="#292830"
          variant="outlined"
          placeholder="Enter your email"
        >
          <template v-slot:append-inner>
            <v-btn
              class="align-center"
              style="width: 102px; height: 48px"
              color="#FF7235"
              variant="flat"
              @click="subscribeAndClear"
            >
              <span class="text-none">
                Subscribe
              </span>
            </v-btn>
          </template>
        </v-text-field>
        <span style="font-size: 14px; line-height: 22px; font-weight: 400; color: #BDBDBD">
          We don’t sell your email and spam
        </span>
      </div>
    </div>
  </div>
  <div class="container" style="margin-bottom: 20px">
    <hr style="border: 1px solid #BDBDBD33; color: #BDBDBD33">
  </div>
  <div class="d-flex justify-space-between" style="width: 1111px; margin: 0 auto; font-size: 14px; line-height: 22px; color: #292830;">
    <div>
      <span>
          Privacy & Terms
      </span>
      <span>
          Contact Us
      </span>
    </div>
    <div>
      <span>
          Copyright @ 2022 xpence
      </span>
    </div>
    <div class="d-flex">
      <v-img style="width: 20px; height: 20px;" src="/facebook_footer.png"></v-img>
      <v-img style="width: 20px; height: 20px; margin-right: 12px; margin-left: 12px;" src="/twitter_footer.png"></v-img>
      <v-img style="width: 20px; height: 20px;" src="/linkedin_footer.png"></v-img>
    </div>
  </div>
</div>
</template>

<style scoped>
</style>

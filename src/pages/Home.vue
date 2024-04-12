<script setup>
import Product from "@/components/Product.vue"; // Путь к файлу Product.vue
import Main from "@/components/Main.vue"; // Путь к файлу Main.vue
import Feature from "@/components/Feature.vue";
import SecondFeature from "@/components/Second-Feature.vue"; // Путь к файлу Brands.vue
import ThirdFeature from "@/components/Third-Feature.vue";
import ProductFeatures from "@/components/Product-Features.vue";
import Plan from "@/components/Plan.vue";
import Testimonial from "@/components/Testimonial.vue";
import Banner from "@/components/Banner.vue";
</script>

<template>
  <v-app>
    <v-row class="wrapper">
      <v-col class="pa-0" cols="12">
        <Main></Main>
      </v-col>
      <v-col class="pa-0" cols="12">
        <Product></Product>
      </v-col>
      <v-col class="pa-0" cols="12">
        <Feature></Feature>
      </v-col>
      <v-col class="pa-0" cols="12">
        <SecondFeature></SecondFeature>
      </v-col>
      <v-col class="pa-0" cols="12">
        <ThirdFeature></ThirdFeature>
      </v-col>
      <v-col class="pa-0" cols="12">
        <ProductFeatures></ProductFeatures>
      </v-col>
      <v-col class="pa-0" cols="12">
        <Plan></Plan>
      </v-col>
      <v-col class="pa-0" cols="12">
        <Testimonial></Testimonial>
      </v-col>
      <v-col class="pa-0" cols="12">
        <Banner></Banner>
      </v-col>
    </v-row>
  </v-app>
</template>

<style scoped>
</style>


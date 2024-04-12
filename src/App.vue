<script setup>
import Header from "@/components/Header.vue";
import Home from "@/pages/Home.vue";
import Footer from "@/components/Footer.vue";
</script>

<template>
  <v-app color="white">
    <v-row class="wrapper ma-auto">
      <v-col class="pa-0" cols="12">
        <div style="height: 48px;">
          <Header></Header>
        </div>
      </v-col>
      <v-col class="pa-0" cols="12">
          <Home></Home>
      </v-col>
      <v-col cols="12">
        <Footer></Footer>
      </v-col>
    </v-row>
  </v-app>
</template>

<style>
.container {
  width: 1109px !important;
  margin: 0 auto;
}
.wrapper {
  width: 1440px !important;
  margin: 0 auto;
}
</style>

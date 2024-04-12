<script setup>

</script>

<template>
    <div class="parent container d-flex">
      <div class="nigga_block">
        <div class="d-flex">
          <span class="font-weight-bold" style="font-size: 96px; color:#292830; line-height: 96px">
            Track your Expenses & Save Money
          </span>
        </div>
        <div class="mt-5 mb-10">
          <span style="color: #BDBDBD; font-size: 24px; line-height: 38px">
            Helps you to organize your income and expenses
          </span>
        </div>
        <div>
          <v-btn
            color="#FF7235"
            variant="flat"
            class="orange-btn rounded-lg text-none mr-6"
          >
            <span style="color:#FFFFFF; font-size: 24px">
              Try free demo
            </span>
            <img src="../assets/icons/arrow.svg" alt="Стрелка" class="ml-2">
          </v-btn>
          <span style="font-size: 24px; color: #BDBDBD; line-height: 38px">
            — Web, iOS and Android
          </span>
        </div>
      </div>

      <div class="d-flex align-center mb-auto">
        <v-img class="illustration" src="/illustration.png"></v-img>
      </div>

    </div>
</template>

<style scoped>
.illustration {
  width: 538px;
  height: 478px;
}

.nigga_block {
  max-width: 540px;
  max-height: 462px;
}

.orange-btn {
  width: 225px !important;
  height: 75px !important;
}

.parent {
  margin-top: 166px;
}
</style>

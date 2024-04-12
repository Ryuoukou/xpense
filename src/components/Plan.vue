<script setup>

</script>

<template>
<div class="wrapper" style="background-color: #FFFAF8">
  <div class="container d-flex flex-column justify-center" style="height: 900px">

    <div class="d-flex justify-center">
          <span class="font-weight-bold" style="font-size: 72px; color:#292830; line-height: 72px">
            Choose your flexible plan.
          </span>
    </div>

    <div class="d-flex justify-space-between" style="margin-top: 80px">

      <div>
        <v-card variant="flat" class="pl-10 d-flex flex-column align-start" width="350" height="500" style="border: 1px solid #F5F5F5">
          <div class="mb-6" style="width: 20px; height: 19px; margin-top: 41px;">
            <v-img src="/backpack.png">

            </v-img>
          </div>
          <div class="mb-6" style="font-weight: 600; font-size: 32px; line-height: 51px">
            <span>
                Starter Plan
            </span>
          </div>
          <div class="galochka_block d-flex flex-column mb-6">
            <span>
              <img class="mr-2" src="/Galochka.png" alt="">Store unlimited data
            </span>
            <span class="mt-2 mb-2">
              <img class="mr-2" src="/Galochka.png" alt="">Export to pdf, xls, csv
            </span>
            <span>
              <img class="mr-2" src="/Galochka.png" alt="">Cloud server support
            </span>
          </div>
          <div class="mb-10">
            <div class="d-flex align-center">
              <span style="font-size: 24px; font-weight: 600; color: #000000; line-height: 38px">
                $9.99/
              </span>
              <span style="font-size: 20px; font-weight: 300; color: #BDBDBD; line-height: 32px">
                year
              </span>
            </div>
            <span style="font-size: 12px; color: #BDBDBD; line-height: 19px">
              up to 3 user + 1.99 per user
            </span>
          </div>
          <div>
            <v-btn width="136" height="50" variant="outlined" rounded-lg style="color: #FF7235" class="text-none">
              <span style="margin-right: 10px">
                Get this
              </span>
              <img src="/big-arrow-right.png" alt="">
            </v-btn>
          </div>
        </v-card>
      </div>

      <div>
        <v-card variant="flat" class="pl-10 d-flex flex-column align-start" width="350" height="500" style="box-shadow: 0 0 50px 0 #0000000A;">
          <div class="mb-6" style="width: 20px; height: 19px; margin-top: 41px;">
            <v-img src="/gift.png">

            </v-img>
          </div>
          <div class="mb-6" style="font-weight: 600; font-size: 32px; line-height: 51px">
            <span>
                Silver Plan
            </span>
          </div>
          <div class="galochka_block d-flex flex-column mb-6">
            <span>
              <img class="mr-2" src="/Galochka.png" alt="">Store unlimited data
            </span>
            <span class="mt-2 mb-2">
              <img class="mr-2" src="/Galochka.png" alt="">Export to pdf, xls, csv
            </span>
            <span>
              <img class="mr-2" src="/Galochka.png" alt="">Cloud server support
            </span>
          </div>
          <div class="mb-10">
            <div class="d-flex align-center">
              <span style="font-size: 24px; font-weight: 600; color: #000000; line-height: 38px">
                $19.99/
              </span>
              <span style="font-size: 20px; font-weight: 300; color: #BDBDBD; line-height: 32px">
                year
              </span>
            </div>
            <span style="font-size: 12px; color: #BDBDBD; line-height: 19px">
              up to 3 user + 1.99 per user
            </span>
          </div>
          <div>
            <v-btn width="136" height="50" variant="flat" rounded-lg color="#FF7235" class="text-none">
              <span style="color: #FFFFFF; margin-right: 10px">
                Get this
              </span>
              <img style="" src="/white-big-arrow-right.png" alt="">
            </v-btn>
          </div>
        </v-card>
      </div>

      <div>
        <v-card variant="flat" class="pl-10 d-flex flex-column align-start" width="350" height="500" style="border: 1px solid #F5F5F5">
          <div class="mb-6" style="width: 20px; height: 19px; margin-top: 41px;">
            <v-img src="/bookmark.png">

            </v-img>
          </div>
          <div class="mb-6" style="font-weight: 600; font-size: 32px; line-height: 51px">
            <span>
                Diamond Plan
            </span>
          </div>
          <div class="galochka_block d-flex flex-column mb-6">
            <span>
              <img class="mr-2" src="/Galochka.png" alt="">Store unlimited data
            </span>
            <span class="mt-2 mb-2">
              <img class="mr-2" src="/Galochka.png" alt="">Export to pdf, xls, csv
            </span>
            <span>
              <img class="mr-2" src="/Galochka.png" alt="">Cloud server support
            </span>
          </div>
          <div class="mb-10">
            <div class="d-flex align-center">
              <span style="font-size: 24px; font-weight: 600; color: #000000; line-height: 38px">
                $29.99/
              </span>
              <span style="font-size: 20px; font-weight: 300; color: #BDBDBD; line-height: 32px">
                year
              </span>
            </div>
            <span style="font-size: 12px; color: #BDBDBD; line-height: 19px">
              up to 3 user + 1.99 per user
            </span>
          </div>
          <div>
            <v-btn width="136" height="50" variant="outlined" rounded-lg style="color: #FF7235" class="text-none">
              <span style="margin-right: 10px">
                Get this
              </span>
              <img src="/big-arrow-right.png" alt="">
            </v-btn>
          </div>
        </v-card>
      </div>

    </div>
  </div>
</div>
</template>

<style scoped>
.galochka_block span {
  font-size: 18px;
  color: #292830;
  line-height: 29px;
}
</style>

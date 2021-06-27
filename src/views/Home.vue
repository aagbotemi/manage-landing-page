<template>
  <div class="body-container">
    <v-container class="jumbotron mt-md-16 mt-3">
      <v-row>
        <v-col order-md="2" md="6" cols="12" class="text-center">
          <img class="jumbotron-image" src="images/illustration-intro.svg">
        </v-col>
        <v-col class="mt-sm-0 mt-n6" order-md="1" md="6" cols="12">
          <h1 class="mb-4">Bring everyone together to build better products.</h1>
          <p>Manage makes it simple for software teams to plan day-to-day tasks while keeping the longer team goals in view.</p>
          <v-btn rounded color="hsl(12, 88%, 59%)" class="white--text text-capitalize">Get Started</v-btn>
        </v-col>
      </v-row>
    </v-container>
    <v-container class="manage-peculiarity mt-12">
      <v-row>
        <v-col class="text-center text-sm-left" md="6" cols="12">
          <h1 class="mb-2">What's different about Manage?</h1>
          <p>Manage provides all the functionality your team needs, without the complexity. Our software is tailor-made for modern digital product teams.</p>
        </v-col>
        <v-col class="d-none d-sm-block" md="6" cols="12">
          <div class="d-flex align-start">
            <span class="px-4 py-1">01</span>
            <div class="ml-3">
              <h4 class="mb-1">Track company-wide progress</h4>
              <p>See how your day-to-day tasks fit into the wider vision.Go from tracking progress at the milestone level all the way done to the smallest of details. Never lose sight of the bigger picture again.</p>
            </div>
          </div>
          <div class="d-flex align-start">
            <span class="px-4 py-1">02</span>
            <div class="ml-3">
              <h4 class="mb-1">Advanced built-in reports</h4>
              <p>Set internal delivery estimates and track progress toward company goals. Our customisable dashboard helps you build out the reports you need to keep key stakeholders informed.</p>
            </div>
          </div>
          <div class="d-flex align-start">
            <span class="px-4 py-1">03</span>
            <div class="ml-3">
              <h4 class="mb-1">Everything you need in one place</h4>
              <p>Stop jumping from one service to another to communicate, store files, track tasks and share documents. Manage offers am all-in-one team productivity solution.</p>
            </div>
          </div>
        </v-col>
        <v-col class="d-sm-none" md="6" cols="12">
          <div>
            <div class="mobile-bg d-flex align-baseline">
              <span class="px-4 py-1">01</span>
              <h4 class="mb-1 ml-3">Track company-wide progress</h4>
            </div>
            <p class="mt-2 ml-2">See how your day-to-day tasks fit into the wider vision.Go from tracking progress at the milestone level all the way done to the smallest of details. Never lose sight of the bigger picture again.</p>
          </div>
          <div>
            <div class="mobile-bg d-flex align-baseline">
              <span class="px-4 py-1">02</span>
              <h4 class="mb-1 ml-3">Advanced built-in reports</h4>
            </div>
            <p class="mt-2 ml-2">Set internal delivery estimates and track progress toward company goals. Our customisable dashboard helps you build out the reports you need to keep key stakeholders informed.</p>
          </div>
          <div class="">
            <div class="mobile-bg d-flex align-baseline">
              <span class="px-4 py-1">03</span>
              <h4 class="mb-1 ml-3">Everything you need in one place</h4>
            </div>
            <p class="mt-2 ml-2">Stop jumping from one service to another to communicate, store files, track tasks and share documents. Manage offers am all-in-one team productivity solution.</p>
          </div>
        </v-col>
      </v-row>
    </v-container>

  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Home'
})
</script>

<style lang="scss">
.jumbotron{
  z-index: 5;
  overflow: hidden;

  h1 {
    font-size: 35px;
  }
  p {
    color: var(--clr-grayish-blue);
    font-size: 18px;
    line-height: 1.4;
  }
  .jumbotron-image {
    width: 22rem;
  }
}
@media only screen and (min-width: 600px) {
  .jumbotron{
    .jumbotron-image {
      width: 30rem;
    }
    h1 {
      font-size: 50px;
    }
  }
  /*.bottom-jumbotron {
    background-image: linear-gradient(
        rgb(242, 95, 98),
        rgb(242, 95, 98)
    ),
    url("./../manage-landing-page/public/images/bg-simplify-section-desktop.svg");
  }*/
}
.manage-peculiarity {
  span {
    background-color: var(--clr-bright-red);
    color: #fff;
    border-radius: 20px;
  }
  .mobile-bg {
    background-color: rgba(242, 95, 98, 0.3);
    border-radius: 14px 0px 0px 14px;
  }
}
</style>

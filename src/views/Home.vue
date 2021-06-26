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
</style>

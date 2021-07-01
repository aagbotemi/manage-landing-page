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

    <div class="testimonial mt-10">
      <h2 class="mb-5 text-center">What they've said</h2>
      <div>
        <VueSlickCarousel class="d-none d-sm-block" v-bind="settings">
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-ali.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Ali Bravo</h4>
              <v-card-text class="text-center pt-0">
                We have been able to cancel so many other subscriptions since using Manage. There is no more cross-channel confusion and everyone is much more focused."
              </v-card-text>
            </v-card>
          </div>
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-richard.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Richard Watts</h4>
              <v-card-text class="text-center pt-0">
                "Manage allows us to provide structure and keeps us organized and focused. I can't stop preaching them to everyone I talk to! The solution provided is superb."
              </v-card-text>
            </v-card>
          </div>
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-anisha.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Anisha Li</h4>
              <v-card-text class="text-center pt-0">
                "Manage has supercharged our team's workflow. The team helps maintain visibility on larger milestones at all times and keeps everyone motivated."
              </v-card-text>
            </v-card>
          </div>
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-shanai.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Shanai Shegantan</h4>
              <v-card-text class="text-center pt-0">
                "Manage allows us to provide structure and keeps us organized. The team helps maintain visibility on larger milestones and keeps everyone motivated."
              </v-card-text>
            </v-card>
          </div>
        </VueSlickCarousel>

        <VueSlickCarousel class="d-sm-none" v-bind="mobileSettings">
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-ali.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Ali Bravo</h4>
              <v-card-text class="text-center pt-0">
                We have been able to cancel so many other subscriptions since using Manage. There is no more cross-channel confusion and everyone is much more focused."
              </v-card-text>
            </v-card>
          </div>
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-richard.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Richard Watts</h4>
              <v-card-text class="text-center pt-0">
                "Manage allows us to provide structure and keeps us organized and focused. I can't stop preaching them to everyone I talk to! The solution provided is superb."
              </v-card-text>
            </v-card>
          </div>
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-anisha.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Anisha Li</h4>
              <v-card-text class="text-center pt-0">
                "Manage has supercharged our team's workflow. The team helps maintain visibility on larger milestones at all times and keeps everyone motivated."
              </v-card-text>
            </v-card>
          </div>
          <div class="pt-5 px-3">
            <v-card class="card mb-8 mt-md-6 text-center text-sm-left">
              <div class="card-img pa-2 text-center">
                <img
                  src="images/avatar-shanai.png"
                />
              </div>
              <h4 class="pt-0 text-center pb-2 mt-n7">Shanai Shegantan</h4>
              <v-card-text class="text-center pt-0">
                "Manage allows us to provide structure and keeps us organized. The team helps maintain visibility on larger milestones and keeps everyone motivated."
              </v-card-text>
            </v-card>
          </div>
        </VueSlickCarousel>

        <div class="d-flex justify-center mt-12 mt-sm-5">
          <v-btn rounded color="hsl(12, 88%, 59%)" class="white--text text-capitalize">Get Started</v-btn>
        </div>

      </div>
    </div>

    <div class="bottom-jumbotron mt-16">
      <v-container class="d-sm-flex text-center text-sm-left py-16">
        <h1>Simplify how your team <br /> works today.</h1>
        <v-spacer />
        <v-btn rounded color="white" class="white deep-orange--text text--accent-2 text-capitalize mt-8 mt-sm-0">Get Started</v-btn>
      </v-container>
    </div>
    <footer class="py-10">
      <v-container>
        <v-row>

          <v-col order-md="4" md="4" cols="12">
            <v-form ref="form" class="d-flex" @submit.prevent="submitEmail"
                    v-model="valid">
              <v-text-field v-model="email"
                            :rules="emailRules" background-color="white" rounded dense hide-details="auto" outlined placeholder="Updates in your inbox" />
              <v-btn rounded color="hsl(12, 88%, 59%)" class="white--text text-capitalize ml-2">Go</v-btn>
            </v-form>
          </v-col>
          <v-col order-md="2" md="2" cols="6">
            <ul class="ml-n6">
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  Home
                </router-link>
              </li>
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  Pricing
                </router-link>
              </li>
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  Products
                </router-link>
              </li>
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  About Us
                </router-link>
              </li>
            </ul>
          </v-col>
          <v-col order-md="3" md="3" cols="6">
            <ul class="ml-n6">
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  Careers
                </router-link>
              </li>
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  Community
                </router-link>
              </li>
              <li class="mb-1">
                <router-link class="text-decoration-none" to="/">
                  Privacy Policy
                </router-link>
              </li>
            </ul>
          </v-col>
          <v-col class="text-center text-md-left" order-md="1" md="3" cols="12">
            <div>
              <img src="/images/logo.svg">
              <div class="mt-7 mt-md-12">
                <a class="mr-4" href="#"
                ><v-icon medium>{{ icons.facebook }}</v-icon></a
                >
                <a class="mr-4" href="#"
                ><v-icon medium>{{ icons.youtube }}</v-icon></a
                >
                <a class="mr-4" href="#"
                ><v-icon medium>{{ icons.twitter }}</v-icon></a
                >
                <a class="mr-4" href="#"
                ><v-icon medium>{{ icons.pinterest }}</v-icon></a
                >
                <a class="mr-4" href="#"
                ><v-icon medium>{{ icons.instagram }}</v-icon></a
                >
              </div>
            </div>
          </v-col>

        </v-row>

        <div class="text-right mt-10 mt-md-3">
          <span >Copyright {{ copyrightYear }}. All Rights Reserved.</span>
        </div>
      </v-container>
    </footer>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
import icons from '@/utils/icons'

export default Vue.extend({
  name: 'Home',
  components: {
    VueSlickCarousel
  },
  data: () => ({
    icons,
    emailArray: [] as Array<any>,
    valid: true,
    email: '',
    emailRules: [
      (email: any) => !!email || 'E-mail is required',
      (email: any) => /.+@.+\..+/.test(email) || 'E-mail must be valid'
    ],
    settings: {
      arrows: false as boolean,
      dots: false as boolean,
      infinite: true as boolean,
      speed: 3700 as number,
      slidesToShow: 3 as number,
      slidesToScroll: 1 as number,
      autoplay: true as boolean,
      autoplaySpeed: 3700 as number,
      cssEase: 'linear' as string
      // "touchThreshold": 5
    },
    mobileSettings: {
      arrows: false as boolean,
      dots: true as boolean,
      infinite: true as boolean,
      speed: 3700 as number,
      slidesToShow: 1 as number,
      slidesToScroll: 1 as number,
      autoplay: true as boolean,
      autoplaySpeed: 3700 as number,
      cssEase: 'linear' as string,
      // "touchThreshold": 5
      dotsClass: 'slick-dots' as string,
      edgeFriction: 0.35 as number
    }
  }),
  methods: {
    reset () {
      this.$refs.form.reset()
    },
    submitEmail () {
      this.reset()
      alert('Email submitted successfully!')
      this.email = ''
    }
  },
  computed: {
    copyrightYear () {
      return new Date().getFullYear()
    }
  }
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

.card {
  background: var(--clr-very-light-gray) !important;
  .card-img {
    transform: translateY(-28px);
    img {
      width: 3.3rem;
    }
  }
}
.bottom-jumbotron {
  background: url("../../public/images/bg-simplify-section-mobile.svg"), var(--clr-bright-red);
  h1 {
    color: var(--clr-very-light-gray);
  }
}
footer {
  background: var(--clr-very-dark-blue);
  color: var(--clr-very-light-gray);

  img {
    filter: brightness(0.9) invert(0.99);
  }

  a {
    .v-icon {
      filter: brightness(1) invert(1);
    }
  }

  ul {
    list-style: none;

    li a{
      color: var(--clr-very-light-gray) !important;
    }
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
  .bottom-jumbotron {
    background: url('../../public/images/bg-simplify-section-desktop.svg'), var(--clr-bright-red)
  }
}
</style>

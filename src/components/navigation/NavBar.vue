<template>
  <v-app-bar app elevation="0" id="nav-bar">
    <v-container class="d-flex align-center">
      <v-app-bar-nav-icon  class="d-md-none" @click="sidebar.drawer = !sidebar.drawer" />
      <v-spacer class="d-md-none"/>
      <img style="z-index: 1" src="images/logo.svg" alt="manage logo" class="mt-2"/>
      <v-spacer class="d-md-flex d-none" />
      <ul class="d-md-flex d-none">
        <li class="mr-4" :key="index"
            v-for="(item, index) in menuItems">
          <router-link class="text-decoration-none" :to="item.url">{{ item.title }}</router-link>
        </li>
      </ul>
      <v-spacer class="d-none d-sm-flex" />
      <!--      <img src="../../../public/images/bg-tablet-pattern.svg" class="tablet-img-top" alt="tablet pattern image">-->
      <v-btn rounded color="hsl(12, 88%, 59%)" class="d-none d-sm-flex white--text text-capitalize">Get Started</v-btn>
    </v-container>
  </v-app-bar>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'nav-bar' as string,
  props: {
    sidebar: Object as () => { drawer: boolean }
  },
  data: () => ({
    menuItems: [
      { title: 'Pricing', url: '/' },
      { title: 'Product', url: '/' },
      { title: 'About Us', url: '/' },
      { title: 'Careers', url: '/' },
      { title: 'Community', url: '/' }
    ] as Array<{title: string, url: any}>
  })
})
</script>

<style scoped lang="scss">
.v-app-bar {
  background-color: white !important;
}
ul {
  list-style: none;

  li a {
    color: var(--clr-dark-blue);
    font-weight: var(--font-weight-md);

    &:hover {
      color: var(--clr-grayish-blue);
    }
  }
}
.tablet-img-top {
  position: absolute;
  right: -30px;
  top: -30px;
  //z-index: 10;
  width: 22rem !important;
}
.v-btn {
  // z-index: 10000 !important;
}
/*.v-app-bar {
  background-color: white !important;
  border-bottom: 1px solid #C3CBD6 !important;

  .v-text-field-slot {
    //height: 30px;
  }
}

.fund-account {
  background: #00B388 0% 0% no-repeat padding-box;
  border: 1px solid #00B388;
  border-radius: 7px;
  color: #FFFFFF;

  &:focus {
    outline: none;
  }
}

.no-background-hover::before {
  background-color: transparent !important;
}
#height {
  max-height: 20px !important;
}
.v-btn--fab.v-size--small {
  height: 30px;
  width: 30px;
  box-shadow: 0px 5px 30px #C3CBD6;

  background: red !important;

  &:hover, &:focus {
    background: transparent !important;
  }

}*/

</style>

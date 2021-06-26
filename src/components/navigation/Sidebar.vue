<template>
    <v-navigation-drawer temporary
                         v-model="sidebar.drawer" app width="221" id="side-bar"
                         :mobile-breakpoint="$vuetify.breakpoint.thresholds.sm"
    >
      <v-icon class="close-icon pa-1" color="#fff" @click="sidebar.drawer = !sidebar.drawer">{{ icons.close }}</v-icon>
      <div class="d-flex flex-column" style="min-height: 100vh">

        <ul class="mt-9">
          <li @click="sidebar.drawer = !sidebar.drawer" class="ml-n4 mr-4 text-center mb-3" :key="index"
              v-for="(item, index) in menuItems">
            <router-link class="text-decoration-none" :to="item.url">{{ item.title }}</router-link>
          </li>
          <li>
            <v-btn style="width: 150px" rounded color="hsl(12, 88%, 59%)" class="d-none d-sm-flex white&#45;&#45;text text-capitalize">Get Started</v-btn>
          </li>
        </ul>
        <div class="mb-4 mx-auto mt-auto">
          <img src="images/logo.svg" alt="anchor logo" />
        </div>
      </div>
    </v-navigation-drawer>
</template>

<script lang="ts">
import Vue from 'vue'
import icons from '@/utils/icons'

export default Vue.extend({
  name: 'sidebar' as string,
  props: {
    sidebar: Object as () => { drawer: boolean }
  },
  data: () => ({
    icons,
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
ul {
  list-style: none;

  li a {
    color: var(--clr-dark-blue);
    font-weight: var(--font-weight-md);
    font-size: 20px;

    &:hover {
       color: var(--clr-grayish-blue);
    }
  }
}
.close-icon {
  background-color: hsl(12, 88%, 59%);
  border-radius: 50%;
  position: absolute;
  right: .7rem;
  top: .7rem;

  &:hover {
    transform: rotate(45deg);
  }
}
</style>

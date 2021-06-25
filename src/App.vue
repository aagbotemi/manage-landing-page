<template>
  <v-app>
    <nav-bar :sidebar="sidebar" />
    <sidebar :sidebar="sidebar" />
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import NavBar from '@/components/navigation/NavBar.vue'
import Sidebar from '@/components/navigation/Sidebar.vue'

export default Vue.extend({
  name: 'App',
  components: {
    Sidebar,
    NavBar
  },
  data: () => ({
    sidebar: {
      drawer: false as boolean
    }
  })
})
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;700&display=swap');

:root {
  /* Primary color */
  --clr-bright-red: hsl(12, 88%, 59%);
  --clr-dark-blue: hsl(228, 39%, 23%);
  /* Neutral */
  --clr-grayish-blue: hsl(227, 12%, 61%);
  --clr-very-dark-blue: hsl(233, 12%, 13%);
  --clr-pale-red: hsl(13, 100%, 96%);
  --clr-very-light-gray: hsl(0, 0%, 98%);

  --font-size: 16px;
  --font-weight: 400;
  --font-weight-md: 500;
  --font-weight-lg: 700;
}

body  {
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
}

h1, h4, h2 {
  color: var(--clr-very-dark-blue);
  line-height: 1.1;
  //
}
p {
  color: var(--clr-grayish-blue);
  line-height: 1.4;
}
</style>

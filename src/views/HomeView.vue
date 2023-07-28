<template>
  <v-app>
    <NavBar/>
    <v-content>
      asdasdsdasdas
      <BanNer/>
      <ItemSLider/>
      <LandingPage msg="Welcome to Your Vue.js App"/>
    </v-content>
  </v-app>
</template>

<script>
// @ is an alias to /src
import LandingPage from '@/components/LandingPage.vue'
import NavBar from '@/components/NavBar.vue'
import BanNer from '@/components/Banner.vue'
import ItemSLider from '@/components/ItemSlider.vue'

export default {
  name: 'HomeView',
  components: {
    LandingPage,
    NavBar,
    BanNer,
    ItemSLider,
  }
}
</script>

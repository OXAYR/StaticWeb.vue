<template>
  <v-app>
    <NavBar/>
    <v-content>
      <BanNer/>
      <ItemSLider/>
      <LowerContent msg="Welcome to Your Vue.js App"/>
    </v-content>
  </v-app>
</template>

<script>
// @ is an alias to /src
import LowerContent from '@/components/LowerContent.vue'
import NavBar from '@/components/NavBar.vue'
import BanNer from '@/components/Banner.vue'
import ItemSLider from '@/components/ItemSlider.vue'

export default {
  name: 'HomeView',
  components: {
    LowerContent,
    NavBar,
    BanNer,
    ItemSLider,
  }
}
</script>

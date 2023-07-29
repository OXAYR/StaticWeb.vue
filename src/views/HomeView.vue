<template>
  <v-app>
    <NavBar/>
    <v-content style="margin-top: 10rem;">
      <BanNer msg=" Cost effective readymade sizes. 
      Choose a frame style then upload your photo and we'll print, build,
      and dispatch your frame the next day. Ideal for quick gifts." header="Standard sizes & gift frames"
      :imageSrc="require('../assets/Banner.png')"
      imageAlt="UpperBanner"/>

      <ItemCard text="Wire-Brushed bare wood" header="Brancaster" 
      :imageSrc="require('../assets/Slide_item.jpg')"
      imageAlt="ItemCard"/>
      <ButtonComp text="Design a custom frame"/>

    <div class="bg-blue-grey-lighten-5">
      <BanNer msg="Cost effective readymade sizes. 
      Choose a frame style then upload your photo and we'll print, 
      build, and dispatch your frame the next day. Ideal for quick gifts." header="Standard sizes & gift frames" 
      :imageSrc="require('../assets/lowerContent.png')"
      imageAlt="LowerBanner" color="bg-blue-grey-lighten-5" />
      
      <ItemCard text="20x30cm textured bare wood frame" header="Small Gift Frame in Brancaster (P)" 
      :imageSrc="require('../assets/Slide_item-2.jpg')"
      imageAlt="ItemCard" price="£34.95"/>
      <ButtonComp text="Shop Standard Frames"/>
      
      <BanNer msg="Want that statement gallery wall without the hassle? 
      Choose one of our gallery walls and upload your photos in minutes, 
      or get one of our designers to help create a truly custom one. Coming soon!" header="Gallery walls" 
      :imageSrc="require('../assets/lowerContent-2.png')"
      imageAlt="LowerBanner2" color="bg-blue-grey-lighten-5"/>
      <ButtonComp text="Coming Soon!"/>
    </div>
    
    </v-content>
    <FooterComp />
  </v-app>
</template>

<script>
// @ is an alias to /src

import NavBar from '@/components/NavBar.vue'
import BanNer from '@/components/Banner.vue'
import ItemCard from '@/components/ItemCard.vue'
import ButtonComp from '@/components/ButtonComp.vue'
import FooterComp from '@/components/FooterComp.vue'

export default {
  name: 'HomeView',
  components: {
    NavBar,
    BanNer,
    ItemCard,
    ButtonComp,
    FooterComp
  }
}
</script>

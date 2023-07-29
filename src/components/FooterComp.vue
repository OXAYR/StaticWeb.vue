<template>
  <v-footer
    class="bg-brown-darken-4"
  >
  <v-container >
      <v-row>
        <v-col
        cols="2"
        >
        <img src="../assets/hang-logo-white.svg" alt="logo" width="100" class="my-10"> 
        <br>
        <img src="../assets/facebook-white.svg" alt="fb-link" width="20" class="ma-2">
        <img src="../assets/insta-white.svg" alt="insta-link" width="20" class="ma-2">
        <img src="../assets/pin-white.svg" alt="pinterest-link" width="20" class="ma-2">  
      </v-col>
      <v-col
        cols="2"
        > 
        <div class="mt-10">
        <p class="text-subtitle-1"><b>START FRAMING</b></p> 
        <p class="text-subtitle-1 mb-1 mt-3">Browse All Frames</p>
        <p class="text-subtitle-1 my-1">Upload a Photo</p>
        <p class="text-subtitle-1 my-1">Frame an original</p>
      </div>
      </v-col>
           
      <v-col
        cols="2"
        > 
        <div class="mt-10">
        <p class="text-subtitle-1"><b>HOW IT WORKS</b></p> 
        <p class="text-subtitle-1 mb-1 mt-3">Materials & sustainability</p>
        <p class="text-subtitle-1 my-1">Pricing</p>
        <p class="text-subtitle-1 my-1">Our story</p>
      </div>
      </v-col>
      
      <v-col
        cols="2"
        > 
        <div class="mt-10">
        <p class="text-subtitle-1"><b>SUPPORT</b></p> 
        <p class="text-subtitle-1 mb-1 mt-3">Our Services</p>
        <p class="text-subtitle-1 my-1">Inspiration</p>
        <p class="text-subtitle-1 my-1">FAQs</p>
        <p class="text-subtitle-1 my-1">Contacts</p>
      </div>
      </v-col>
      
      <v-col
        cols="4"
        > 
        <div class="mt-10">
        <p class="text-subtitle-1"><b>SIGN UP FOR EMAIL UPDATES</b></p>
        </div>
      </v-col>
      </v-row>
      </v-container>
  </v-footer>
</template>
  
<script>
export default {
  name:'FooterComp',
  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-instagram',
    ],
  }),
}
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
  
  </style>
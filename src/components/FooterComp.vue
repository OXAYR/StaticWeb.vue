<template>
  <v-footer class="bg-black">
    <v-container>
      <v-row class="d-flex flex-wrap">
        <v-col cols="6" sm="3" md="2">
          <img src="../assets/hang-logo-white.svg" alt="logo" width="100" class="my-10"> 
          <br>
          <img src="../assets/facebook-white.svg" alt="fb-link" width="20" class="ma-2">
          <img src="../assets/insta-white.svg" alt="insta-link" width="20" class="ma-2">
          <img src="../assets/pin-white.svg" alt="pinterest-link" width="20" class="ma-2">  
        </v-col>
        <v-col cols="6" sm="3" md="2">
          <div class="my-10">
            <p class="text-subtitle-1"><b>START FRAMING</b></p> 
            <p class="text-subtitle-1 mb-1 mt-3">Browse All Frames</p>
            <p class="text-subtitle-1 my-1">Upload a Photo</p>
            <p class="text-subtitle-1 my-1">Frame an original</p>
          </div>
        </v-col>
        <v-col cols="6" sm="3" md="2">
          <div class="my-10">
            <p class="text-subtitle-1"><b>HOW IT WORKS</b></p> 
            <p class="text-subtitle-1 mb-1 mt-3">Materials & sustainability</p>
            <p class="text-subtitle-1 my-1">Pricing</p>
            <p class="text-subtitle-1 my-1">Our story</p>
          </div>
        </v-col>
        <v-col cols="6" sm="3" md="2">
          <div class="my-10">
            <p class="text-subtitle-1"><b>SUPPORT</b></p> 
            <p class="text-subtitle-1 mb-1 mt-3">Our Services</p>
            <p class="text-subtitle-1 my-1">Inspiration</p>
            <p class="text-subtitle-1 my-1">FAQs</p>
            <p class="text-subtitle-1 my-1">Contacts</p>
          </div>
        </v-col>
        <v-col cols="12" sm="12" md="4">
          <div class="my-10">
            <p class="text-subtitle-1"><b>SIGN UP FOR EMAIL UPDATES</b></p>
            <v-text-field class="my-5" placeholder="Enter Email">
              <v-btn variant="plain">
                Submit
              </v-btn>
            </v-text-field>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
  <v-footer>
      <p class="text-overline">© 2021 Hang Framing Ltd</p>
  </v-footer>
</template>

  
<script>
export default {
  name:'FooterComp',
}
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">

  </style>
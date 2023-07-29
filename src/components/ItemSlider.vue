<template>
   <v-container>
    <v-row>
      <v-col align-self="center"
        v-for="n in 4"
        :key="n"
        cols="4"
        sm="12"
        md="3"
      >
        <v-card class="ma-4 pa-4 text-left rounded lighten-4" :elevation="3">
          <img src="../assets/Slide_item.jpg" alt="slider" class=" w-100">
          <h3 >Brancasting</h3>
          <p>Wire-brushed bare wood</p>
        </v-card>
      </v-col>
    </v-row>
    </v-container>
  </template>
  <script></script>
  
  <script>
  export default {
    name: 'ItemSlider',
    
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
  
  </style>
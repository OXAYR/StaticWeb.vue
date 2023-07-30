<template>
  <div class="d-none d-md-flex ">
    <v-container>
      <v-row>
        <v-col
          v-for="n in 4"
          :key="n"
          cols="4"
          sm="12"
          md="3"
        >
          <v-card class="ma-4 pa-4 text-left rounded lighten-4" :elevation="3">
            <img :src="imageSrc" :alt="imageAlt" class=" w-100">
            <h3 >{{ header }}</h3>
            <span v-show="price" style="color: darkred;">{{ price }}</span>
            <p>{{ text }}</p>
          </v-card>
        </v-col>
      </v-row>
      </v-container>
    </div>
    <div class="d-md-none">
    <v-sheet
      class="mx-auto"
      max-width="700"
    >
      <v-slide-group
        show-arrows
        
      >
        <v-slide-group-item
          v-for="n in 4"
          :key="n"
        >
        <v-card class="ma-4 pa-4 text-left rounded lighten-4" :elevation="3" style="max-width: 300px;">
            <img :src="imageSrc" :alt="imageAlt" class=" w-100" style="max-height: 200px;">
            <h3 >{{ header}}</h3>
            <span v-show="price" style="color: darkred;">{{ price }}</span>
            <p>{{ text }}</p>
          </v-card>
        </v-slide-group-item>
      </v-slide-group>
    </v-sheet>
    </div>
  </template>
  <script>
  export default {
    name: 'ItemCard',
    props:{ 
      header: {
        type: String,
        required: true,
      },
      text: {
        type: String,
        required: true,
      },
      imageSrc: {
        type: String,
        required: true,
      },
      imageAlt: {
        type: String,
        required: true,
      },
      price: String,
    },
    date(){
      return {
        height: Number,
      }
    },

    methods:{
      gethieght(){
        console.log( screen.width)
      }
    }
    
    
  }
  </script>
  
  
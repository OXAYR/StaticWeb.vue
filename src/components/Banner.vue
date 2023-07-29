<template>
    <v-container >
      <v-row>
        <v-col align-self="center" cols=6>
          <v-sheet class="ma-4 pa-4 text-left text-wrap">
            <h1 class="text-h4 text-medium">{{ header }}</h1>
            <p class="text-subtitle-1">{{ msg }}</p>
          </v-sheet>
        </v-col>
        <v-col cols=6>
          <v-sheet class="ma-2 pa-2 wrap">
            <img :src="imageSrc" :alt="imageAlt" class="w-100 h.auto">
          </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    name: 'BanNer',
    props: {
      msg: {
        type: String,
        required: true,
      },
      header: {
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
    },
  };
  </script>

<template>
  <div >
  <v-container >
        <v-row >
          <v-col  align-self="center" cols=6>
            <v-sheet class="ma-4 pa-4 text-left text-wrap " :class="color">
              <h1 class="text-h4 text-medium">{{ header }}</h1>
              <p class="text-subtitle-1">{{ msg }}</p>
            </v-sheet>
          </v-col>
          <v-col cols=6>
            <v-sheet class="ma-2 pa-2 wrap" :class="color">
              <img :src="imageSrc" :alt="imageAlt" class="w-100 h.auto">
            </v-sheet>
          </v-col>
        </v-row>
      </v-container>
    </div>
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
      color:{
        type: String,
        default: 'bg-white'
      }
    },
  };
  </script>
<style scoped>
/* Other component styles... */
</style>
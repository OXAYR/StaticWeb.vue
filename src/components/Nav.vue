<template>
    <v-card>
      <v-layout>
         <v-app-bar
          color="primary"
          prominent
        >
          <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
  
          <v-toolbar-title > Hang</v-toolbar-title>
  
          <v-spacer></v-spacer>
<!--   
          <v-btn variant="text" icon="mdi-magnify"></v-btn>
  
          <v-btn variant="text" icon="mdi-filter"></v-btn>
  
          <v-btn variant="text" icon="mdi-dots-vertical"></v-btn> -->
        </v-app-bar>
  
        
        <!-- <v-main style="height: 500px;">
          <v-card-text>
            The navigation drawer will appear from the bottom on smaller size screens.
          </v-card-text>
        </v-main> -->
      </v-layout>
    </v-card>
  </template>
  <script>
    export default {
        name: 'NavBar',
  
    }
  </script>
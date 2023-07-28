<template>
   <v-toolbar :elevation="4" color="white" height="100">
    <v-btn variant="plain">
      <span>
      Start Framing
      </span>
    </v-btn>
    <v-btn variant="plain">
      <span>
      How it works
      </span>
    </v-btn>
    <v-spacer>
    <v-toolbar-title >
      <span  class="font-weight-regular text-h4">Hang
      </span>
      </v-toolbar-title>
      </v-spacer>
      <v-btn variant="plain">
      <span>
      Support
      </span>
    </v-btn>
    
    <v-btn variant="plain">
      <v-icon
      size="large"
      color="blue-darken-2"
      icon="mdi-message-text"
    ></v-icon>
    </v-btn>
    </v-toolbar>
  </template>
  <script>
    export default {
        name: 'NavBar',
  
    }
  </script>
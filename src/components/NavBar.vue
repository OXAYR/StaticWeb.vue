<template>
   <v-app-bar :elevation="4" color="white" height="100" >
    <v-btn class="ml-10" variant="plain">
      <span >
      Start Framing
      </span>
    </v-btn>
    <v-btn variant="plain" class="mx-4">
      <span>
      How it works
      </span>
    </v-btn>
    <v-spacer></v-spacer>
    <v-toolbar-title>
      <img src="../assets/hank-logo.svg" alt="hank.logo" width="125" style="margin-right:95px ;" >
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn variant="plain">
      <span>
      Support
      </span>
    </v-btn>
    <v-btn class="mx-4" density="default" icon="mdi-shopping"></v-btn>
    <v-btn class="mr-10" density="default" icon="mdi-account"></v-btn>
    </v-app-bar>
  </template>
  <script>
    export default {
        name: 'NavBar',
  
    }
  </script>
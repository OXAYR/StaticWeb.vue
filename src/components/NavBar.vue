<template>
 
 <div>
  <v-container>
   <v-app-bar :elevation="4" color="white" height="100" >
    <v-app-bar-nav-icon class=" d-md-none"/>
    <v-btn class="d-none d-md-flex" variant="plain">
      Start Framing
    </v-btn>
    <v-btn  variant="plain" class=" d-none d-md-flex">
      How it works
    </v-btn>
    <v-toolbar-title >
      <img class="mr-10" src="../assets/hank-logo.svg" alt="hank.logo" width="125" >
      </v-toolbar-title>
      <v-btn class=" d-none d-md-flex" variant="plain">
      Support
    </v-btn>
    <v-btn density="default" icon="mdi-shopping"></v-btn>
    <v-btn class="mr-10 d-none d-md-flex" density="default" icon="mdi-account"></v-btn>
    </v-app-bar>
  </v-container>
    </div>
  </template>
  <script>
    export default {
        name: 'NavBar',
  
    }
  </script>
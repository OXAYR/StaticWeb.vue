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
    <v-toolbar-title>
      <img src="../assets/hank-logo.svg" alt="hank.logo" width="125" height="125" style="margin-right: 90px;">
      </v-toolbar-title>
      <v-btn variant="plain">
      <span>
      Support
      </span>
    </v-btn>
    <v-btn variant="plain">
      <v-icon
      size="large"
      color="black"
      icon="mdi-shopping"
    ></v-icon>
    </v-btn>
    <v-btn variant="plain">
      <v-icon
      size="large"
      color="black"
      icon="mdi-account"
    ></v-icon>
    </v-btn>
    </v-toolbar>
  </template>
  <script>
    export default {
        name: 'NavBar',
  
    }
  </script>
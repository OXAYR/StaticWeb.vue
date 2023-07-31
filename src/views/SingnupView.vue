<template>
    <div class="SignUp">
      <SignUp/>
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import SignUp from '../components/Signup.vue'
  
  export default {
    name: 'SignUpView',
    components: {
      SignUp
    }
  }
  </script>
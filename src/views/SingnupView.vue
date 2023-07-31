<template>
    <div class="SignUp">
      <SignUpForm/>
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import SignUpForm from '../components/SignupForm.vue'
  
  export default {
    name: 'SignUpView',
    components: {
      SignUpForm
    }
  }
  </script>
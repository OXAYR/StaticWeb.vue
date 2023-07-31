<template>
  <v-sheet width="300" class="mx-auto">
    <v-form >
      <v-text-field
        v-model="firstName"
        label="First name"
      ></v-text-field>
      <v-text-field
        v-model="lastName"
        label="Last name"
      ></v-text-field>
    </v-form>
  </v-sheet>
</template>
<script>
import router from '@/router';
    export default {
  name: 'LoginForm',
  props: {
      msg: String,
    },
  data() {
    return {
        validCredential: false,
        formLogin :{
        email: "",
        password: ''    
        },
        error:[],
    }
},
methods:{
  
    toValidate(obj){
      
          if(localStorage.getItem("Email") == obj.email){
           
            if(localStorage.getItem("Password") == obj.password){
            
              router.push('/todos')
            }
          }
      },
    // Valid: function(obj) {
    //     this.error = [];
    //     const passwordPattern = /^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#$%^&*()_+{}\[\]:;<>,.?~\\/\-='|"])[a-zA-Z0-9!@#$%^&*()_+{}\[\]:;<>,.?~\\/\-='|"']{8,}$/;
    //     const emailPattern = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;

        
    //   if (!emailPattern.test(obj.email)) {
    //     this.error.push("Invalid Email");
    //   } 
    //   if (!passwordPattern.test(obj.password)) {
    //       this.error.push("Invalid Password");
    //   }
        
    //   }
    
    }
    }

</script>

<style scoped>
fieldset{
  margin-bottom: 2rem;
}
.Button{

  margin-top: 2rem;
}
</style>

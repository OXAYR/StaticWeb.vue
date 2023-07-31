<template>
  <form @submit.prevent="submit">
    <v-text-field
      v-model="name.value.value"
      :counter="10"
      :error-messages="name.errorMessage.value"
      label="Name"
    ></v-text-field>

    <v-text-field
      v-model="phone.value.value"
      :counter="7"
      :error-messages="phone.errorMessage.value"
      label="Phone Number"
    ></v-text-field>

    <v-text-field
      v-model="email.value.value"
      :error-messages="email.errorMessage.value"
      label="E-mail"
    ></v-text-field>

    <v-select
      v-model="select.value.value"
      :items="items"
      :error-messages="select.errorMessage.value"
      label="Select"
    ></v-select>

    <v-checkbox
      v-model="checkbox.value.value"
      :error-messages="checkbox.errorMessage.value"
      value="1"
      label="Option"
      type="checkbox"
    ></v-checkbox>

    <v-btn
      class="me-4"
      type="submit"
    >
      submit
    </v-btn>

    <v-btn @click="handleReset">
      clear
    </v-btn>
  </form>
</template>
<script setup>
  import { ref } from 'vue'
  import { useField, useForm } from 'vee-validate'

  const { handleSubmit, handleReset } = useForm({
    validationSchema: {
      name (value) {
        if (value?.length >= 2) return true

        return 'Name needs to be at least 2 characters.'
      },
      phone (value) {
        if (value?.length > 9 && /[0-9-]+/.test(value)) return true

        return 'Phone number needs to be at least 9 digits.'
      },
      email (value) {
        if (/^[a-z.-]+@[a-z.-]+\.[a-z]+$/i.test(value)) return true

        return 'Must be a valid e-mail.'
      },
      select (value) {
        if (value) return true

        return 'Select an item.'
      },
      checkbox (value) {
        if (value === '1') return true

        return 'Must be checked.'
      },
    },
  })
  const name = useField('name')
  const phone = useField('phone')
  const email = useField('email')
  const select = useField('select')
  const checkbox = useField('checkbox')

  const items = ref([
    'Item 1',
    'Item 2',
    'Item 3',
    'Item 4',
  ])

  const submit = handleSubmit(values => {
    alert(JSON.stringify(values, null, 2))
  })
</script>
  
  <script>
  import router from '@/router'
  export default {
    name: 'SignUp',
    props: {
      msg: String,
    },
    
    data() {
      return {
        form : { 
        username: '',
        email: '',
        password: '',
        confrimPassword:'',
        },
        error:[]
        
      }
    },
    computed: {
    // shouldNavigate() {
    //   // Compute the condition based on the form data
    //   return this.getForm(this.form) && this.Validate(this.form);
    // },
  },
    methods: {
      toStore(obj){
        if(obj.email !== "" && obj.password !=="" && obj.username !== "" && obj.confrimPassword!==""){
   
          localStorage.setItem("Username",obj.username)
          localStorage.setItem("Password",obj.password)
          localStorage.setItem("Email",obj.email)
          router.push('/')
        }
      },
  Validate: function(obj) {
        this.error = [];
        const usernamePattern = /^(?=.*[0-9!@#$%^&*()_+{}\[\]:;<>,.?~\\/\-='|"'])\S+$/;
        const passwordPattern = /^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#$%^&*()_+{}\[\]:;<>,.?~\\/\-='|"])[a-zA-Z0-9!@#$%^&*()_+{}\[\]:;<>,.?~\\/\-='|"']{8,}$/;
        const emailPattern = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;

        if (obj.username !== "" && !usernamePattern.test(obj.username)) {
          this.error.push("Invalid Name");
        } 
        if (obj.password !== "" && !passwordPattern.test(obj.password)) {
          this.error.push("Invalid Password");
        } 
        if(obj.password !== obj.confrimPassword){
           this.error.push("Password Does not match")
        }
        if (obj.email !== "" && !emailPattern.test(obj.email)) {
        this.error.push("Invalid Email");
        }
        // } else {
        //   alert("Your credentials have been added successfully!");
        // }
    },

    
    created() {
      // Initialization code javascript load
      console.log('Created');
  
    },
    mounted(){
      // Code that runs when the component is inserted into the DOM html loaded
      console.log('mounted');
    },
    updated() {
      // Code that runs when the component's data or props change
      console.log('updated');
      
    },
    unmounted() {
      // Code that runs when the component is about to be destroyed
      console.log('unmounted');
    },
  }
}
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  /* h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  } */
  
  fieldset{
    margin-bottom: 2rem;
  }
  .Button{
  
    margin-top: 2rem;
  }
  </style>
  
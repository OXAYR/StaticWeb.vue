<template>
  <v-app>
  <NavBar/>
  <router-view/>
  <FooterComp/>
</v-app>
  <!-- <nav> -->
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    
  </nav> -->
</template>
<script>
import NavBar from "./components/NavBar.vue";
import FooterComp from "./components/FooterComp.vue";


export default{
  components:{
    NavBar,
    FooterComp
  }
}

</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

<template>
    <v-content>
        <v-btn class="ma-7 bg-yellow-lighten-3" elevation="0" rounded="xl" size="x-large" >
            <span class="text-button pa-2"> {{ text }}</span></v-btn>
    </v-content>    
</template>
<script>
    export default {
        name: "ButtonComp",
        props:{
            text :{
                type: String,
                required: true,
            }
        }
    }
</script>

<style scoped>
/* .custom-button:{
    color: black;
} */
</style>
<template>
    <v-content>
        <v-btn class="ma-7 text-none" variant="tonal" rounded="xl" size="x-large" color="yellow-darken-4" >{{ text }}</v-btn>
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
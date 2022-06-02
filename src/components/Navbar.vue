<template>
    <v-app-bar app color="white">
        <v-badge color="primary" dot>
            <v-avatar size="50">
                <v-icon x-large color="primary">mdi-cart</v-icon>
            </v-avatar>
        </v-badge>
        <v-toolbar-title class="ml-4">
            <strong>e<span class="green--text">C</span>ommerce</strong>
        </v-toolbar-title>
       
       <v-spacer></v-spacer>
    
        <v-badge  color="#ff0059" overlap content="2" class="mr-2 mt-1">
            <v-avatar color="#ecf7ee" size="40">
                <v-icon x-middle color="#cc2a33">mdi-heart</v-icon>
            </v-avatar>
        </v-badge>
        <v-badge  color="#ff0059" overlap content="3" class="mr-2 mt-1">
            <v-avatar color="#ecf7ee" size="40">
                <v-icon x-middle color="#cc2a33">mdi-shopping</v-icon>
            </v-avatar>
        </v-badge>
        <div class="d-flex flex-column justify-contet text-center">
            <v-avatar class="mx-auto">
                <v-img src="/profile.jpg"></v-img>
            </v-avatar>
           <span class="success--text ml-2">Hi <strong>Ibrahim</strong></span>
        </div>
            <v-icon color="success">mdi-chevron-double-down</v-icon>
    </v-app-bar>
</template>
<script>
export default {

}
</script>
<style scoped>
.v-toolbar__title{font-size:2rem !important;}
</style>
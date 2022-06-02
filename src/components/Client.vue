<template>
    <v-row class="d-flex">
        <v-col cols="12"  sm="12" xs="12" md="4" v-for="(client,i) in clients" :key="i">
           <v-card
               class="elevation-16 mx-auto"
               width="300"
           >
               <v-list subheader two-line>
                   <v-list-item>
                       <v-list-item-avatar>
                           <v-img :src="client.image" loading="lazy"></v-img>
                       </v-list-item-avatar>
                       <v-list-item-content>
                           <v-list-item-title>{{client.name}}</v-list-item-title>
                           <v-list-item-subtitle>{{client.subtitle}}</v-list-item-subtitle>
                       </v-list-item-content>
                   </v-list-item>
               </v-list>
               <v-card-text>
                   {{client.bio}}
               <div class="text-center mt-12">
                   <v-rating
                    v-model="rating"
                   color="yellow darken-3"
                   background-color="grey darken-1"
                   empty-icon="$ratingFull"
                   half-increments
                   hover
                   large
                    ></v-rating>
               </div>
               </v-card-text>
               <v-divider></v-divider>
               <v-card-actions class="justify-space-between">
               <v-btn text>
                    No Thanks
               </v-btn>
               <v-btn
                    color="primary"
                    text
               >
                    Rate Now
               </v-btn>
    </v-card-actions>
  </v-card>
        </v-col>
    </v-row>
</template>
<script>
export default {
    data:()=>({
        rating:3.5,
        clients:[
            {
                name:'Veronika',
                subtitle:'Development Manager',
                image:'client-1.jpg',
                bio:'If you enjoy using Vuetify, please take a few seconds to rate your experience with the framework. It really helps!'
            },
            {
                name:'Jhon',
                subtitle:'CEO',
                image:'client-2.jpg',
                bio:'If you enjoy using Vuetify, please take a few seconds to rate your experience with the framework. It really helps!'
            },
            {
                name:'Alex',
                subtitle:'Software Engineer',
                image:'client-3.jpg',
                bio:'If you enjoy using Vuetify, please take a few seconds to rate your experience with the framework. It really helps!'
            }
        ]
    }),
}
</script>
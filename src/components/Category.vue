<template>
    <v-item-group mandatory class="mt-n8">
        <v-container>
            <v-row justify="center" class="space">
                <v-col cols="12" xs="12" sm="12" md="2" v-for="(category,i) in categories" :key="i">
                    <v-item v-slot="{active,toggle}">
                        <v-card flat dark :color='active?"warning":"white"'
                        :class="active?'borderme' : 'borderout'"
                        class="d-flex justify-center align-center rounded"
                        @click="toggle" hieght="200" outlined
                    >
                    <v-row>
                        <v-col cols="12">
                            <v-list-item three-line>
                             <v-list-item-content class="text-center">
                               <div class="d-inline mx-auto">
                                   <v-img class="mx-auto photo" 
                                   :src="category.image" max-height="100" contain></v-img>
                               </div>
                               <v-list-item-title class="black--text mt-4">
                                   {{ category.title }}
                               </v-list-item-title>
                               <v-list-item-subtitle class="black--text mt-2">
                                 consectetur adipiscing elit.
                               </v-list-item-subtitle>
                             </v-list-item-content>
                           </v-list-item>   
                        </v-col>
                    </v-row>
                    </v-card>
                    </v-item>
                </v-col>
            </v-row>
        </v-container>
    </v-item-group>
</template>
<script>
export default {
    name:'category',
    data: () => ({
        active:false,
        toggle:true,
        categories:[
            {title:'Bag & Wallet',image:'C1.jpg'},
            {title:'Watches',image:'C2.jpg'},
            {title:'Eyewear',image:'C3.jpg'},
            {title:'Basics',image:'C4.jpg'},
            {title:'Jewelry',image:'C5.jpg'},
            {title:'Scarves & Wraps',image:'C6.jpg'},
        ]
    })
}
</script>
<style scoped>
.photo{height:150px;width:150px;}
</style>
<template>
  <v-container>
      <v-item>
    <v-row class="mx-auto">
        <v-col class="d-flex" cols="12" xs="12" sm="6" md="2" v-for="(sport,i) in sports" :key="i">
            <v-card class="mx-auto ml-8 rounded-xl" flat outlined width="300">
                    <div class="justify-center text-center">
                        <v-img :src="sport.image" loading="lazy" height="300" max-width="300" contain></v-img>
                    </div>
                <v-card-title class="black--text">{{ sport.title }}</v-card-title>
                <v-card-subtitle class="grey--text">{{ sport.desc }}</v-card-subtitle>
                <v-card-subtitle class="text-h6 green--text">{{ sport.price }}</v-card-subtitle>
            </v-card>
        </v-col>
    </v-row>
  </v-item>
  </v-container>
</template>
<script>
export default {
    data:()=> ({
        sports:[
            {title:"Testa Toro Men's Slip On - Testa Toro Microfiber...",image:'s1.jpg',desc:'Testa Toro',price:'155 $'},
            {title:"Testa Toro Men's Daily Life Microfiber Casual",image:'s2.jpg',desc:'Testa Toro',price:'159 $'},
            {title:"Testa Toro Men's Embroidered Low Top",image:'s3.jpg',desc:'Testa Toro',price:'125 $'},
            {title:'Desert 2057 - Men Minimalist Lace-Up Flat',image:'s4.jpg',desc:'Desert',price:'119 $'},
            {title:'reebok shoes',image:'s5.jpg',desc:'Reebok',price:'619 $'},
            {title:'Basic Lace-up Sneakers For Men',image:'s6.jpg',desc:'Generic',price:'149 $'},
        ]
    }),
}
</script>
<style lang="css" scoped>
.v-card-title{white-space:1px;}
</style>
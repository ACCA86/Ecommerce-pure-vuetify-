<template>
  <v-container>
      <v-item>
    <v-row class="mx-auto">
        <v-col class="d-flex" cols="12" xs="12" sm="6" md="2" v-for="(shoe,i) in shoes" :key="i">
            <v-card class="mx-auto ml-8 rounded-xl" flat outlined width="300">
                    <div class="justify-center text-center">
                        <v-img :src="shoe.image" loading="lazy" max-height="300" max-width="300" contain></v-img>
                    </div>
                <v-card-title class="black--text">{{ shoe.title }}</v-card-title>
                <v-card-subtitle class="grey--text">{{ shoe.desc }}</v-card-subtitle>
                <v-card-subtitle class="text-h6 green--text">{{ shoe.price }} $</v-card-subtitle>
            </v-card>
        </v-col>
    </v-row>
  </v-item>
  </v-container>
</template>
<script>
export default {
    data:()=> ({
        shoes:[
            {title:"Testa Toro Men's Slip On - Testa Toro Microfiber...",image:'sh1.jpg',desc:'Testa Toro',price:'155'},
            {title:"Testa Toro Men's Daily Life Microfiber Casual",image:'sh2.jpg',desc:'Testa Toro',price:'159'},
            {title:"Testa Toro Men's Embroidered Low Top",image:'sh3.jpg',desc:'Testa Toro',price:'125'},
            {title:'Desert 2057 - Men Minimalist Lace-Up Flat',image:'sh4.jpg',desc:'Desert',price:'119'},
            {title:'reebok shoes',image:'sh5.jpg',desc:'Reebok',price:'619'},
            {title:'Basic Lace-up Sneakers For Men',image:'sh6.jpg',desc:'Generic',price:'149'},
        ]
    }),
}
</script>
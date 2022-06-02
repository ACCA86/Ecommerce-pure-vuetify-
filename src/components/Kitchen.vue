<template>
  <v-container>
      <v-item>
    <v-row class="mx-auto space px-16" justify="center">
        <v-col  cols="12" xs="12" sm="6" md="2"  v-for="(product,i) in products" :key="i" >
            <v-card class=" ml-10 rounded-xl" flat outlined width="400">
                    <div class="justify-center text-center">
                        <v-img :src="product.image" loading="lazy" height="300" max-width="400" contain></v-img>
                    </div>
                <v-card-title class="black--text">{{ product.title }}</v-card-title>
                <v-card-subtitle class="grey--text">{{ product.desc }}</v-card-subtitle>
            </v-card>
        </v-col>
    </v-row>
  </v-item>
  </v-container>
</template>
<script>
export default {
    data:()=> ({
        products:[
            {title:'Mienta CM31316A Barista Coffee Maker, 600 Watt - Black',image:'k1.jpg',desc:'Mienta'},
            {title:'Tornado TST700 Sandwitch Maker 3X1…',image:'k2.jpg',desc:'kitchen Essentials'},
            {title:'MI Electric Hand Blender Mixer Hand-held Egg Beater Mixer, White',image:'k3.jpg',desc:'kitchen Essentials'},
            {title:"Kenwood HFP90 Multifunction kHealthy Air Fryer Oven, 2000W, 11L Capacity - Rose Gold ( International Warranty )",image:'k4.jpg',desc:'kitchen Essentials'},
            {title:'Braun MultiQuick 5 Vario Hand Blender with Attachments, 1000 Watt, White/Grey - MQ 5245 WH',image:'k5.jpg',desc:'kitchen Essentials'},
            {title:'Black & Decker DCM25N-B5 Coffee Maker, Black - 1 Cup',image:'k6.jpg',desc:'kitchen Essentials'},
        ]
    }),
}
</script>
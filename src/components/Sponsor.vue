<template>
   <v-row class="d-flex px-16 mt-10">
       <v-col cols="3" v-for="(partner,i) in partners" :key="i">
           <div class="text-center justify-center">
               <v-img :src="partner.img" contain height="250"></v-img>
           </div>
       </v-col>
   </v-row>
</template>
<script>
export default {
    data:()=>({
        partners:[
            {img:'gd.png'},{img:"adidas.png"},{img:"lacoste.png"},{img:"airbnb.png"}
        ]
    }),
}
</script>
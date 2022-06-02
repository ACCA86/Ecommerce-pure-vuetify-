<template>
  <v-app>
    <Navbar />
    <v-container fluid>
      <v-row>
        <v-col cols="12">
          <v-card class="mx-auto rounded" flat>
           <v-img src="shopping.jpg" loading="lazy" max-height="100%" max-width="100%" contain>
              <v-card-title class="top ml-10">
                <h2>Your Order</h2>
              </v-card-title>
              <v-card-title class="ml-10 mt-n8">
                <h2>Daily Here</h2>
              </v-card-title>
              <v-card-text class="">
                <v-row>
                  <v-col cols="2" ms="4" sx="3">
                    <v-text-field label="Search" filled solo prepend-inner-icon="mdi-magnify" 
                    flat rounded outlined success
                    ></v-text-field>
                  </v-col>
                  <v-col cols="2" class="marginLeft">
                    <v-btn color="green" rounded dark x-large class="py-7 d-nonw d-sm-none d-md-flex">Search</v-btn>
                  </v-col>
                </v-row>
              </v-card-text>
            </v-img>
          </v-card>
          <v-toolbar flat color="transparent">
            <v-toolbar-title class="text-h6">Category</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn-toggle v-model="toggle" group color="success">
            <v-btn>
              <v-icon>mdi-chevron-left</v-icon>
            </v-btn>
            <v-btn>
              <v-icon>mdi-chevron-right</v-icon>
            </v-btn>
            </v-btn-toggle>
          </v-toolbar>
          <Category class="py-12" />
          <v-toolbar flat color="transparent">
            <v-toolbar-title class="text-h6">Kitchen</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn rounded dark color="green">
              See More
            </v-btn>
          </v-toolbar>
          <Kitchen />
          <v-toolbar flat>
            <v-toolbar-title class="text-h6">Sports</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn-toggle v-model="toggle" group color="success">
              <v-btn class="cursor-pointer">
                <v-icon>mdi-chevron-left</v-icon>
              </v-btn>
              <v-btn class="cursor-pointer">
                <v-icon>mdi-chevron-right</v-icon>
              </v-btn>
            </v-btn-toggle>
          </v-toolbar>
          <Sport />
          <v-toolbar flat color="transparent">
            <v-toolbar-title class="text-h6">Shoes</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn-toggle v-model="toggle" group color="primary">
              <v-btn>
                <v-icon>mdi-chevron-left</v-icon>
              </v-btn>
              <v-btn>
                <v-icon>mdi-chevron-right</v-icon>
              </v-btn>
            </v-btn-toggle>
          </v-toolbar>
          <Shoes />
          <v-toolbar flat color="transparent">
            <v-toolbar-title class="text-h4">Clients</v-toolbar-title>
          </v-toolbar>
          <Client />
          <v-toolbar flat color="transparent" class="mt-8">
            <v-toolbar-title class="text-h4">Our Trusted Partner</v-toolbar-title>
          </v-toolbar>
          <Sponsor />
           <v-card flat color="#E2F2E5" class="rounded-xl mtob mbottom mx-10 pa-4 con-mobile"
            height="550">
            <v-row>
              <v-col cols="12" xs="12" sm="12" md="5">
                <v-card class="rounded-xl mt-12 ml-16 mobile" outlined flat 
                height="450" width="200">
                  <v-img src="mobile.png"></v-img>
                </v-card>
              </v-col>
              <v-col cols="12" sm="12" xs="12" md="7">
                <h1 class="mt-6 mb-4">Download App</h1>
                <p>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
                  sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
                  Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
                  Excepteur sint occaecat cupidatat non proident, 
                  sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
                <v-btn color="black" dark class="mb-10">
                  <v-icon class="mr-2" color="white">mdi-apple</v-icon>
                   App Store
                </v-btn>
                <v-btn color="black" dark class="mb-10 ml-4">
                  <v-icon class="mr-2" color="white">mdi-google-play</v-icon>
                   App Play
                </v-btn>
              </v-col>
            </v-row>
           </v-card>
          <Footer />
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Category from '@/components/Category.vue'
import Kitchen from '@/components/Kitchen.vue'
import Sport from '@/components/Sport.vue'
import Shoes from '@/components/Shoes.vue'
import Client from '@/components/Client.vue'
import Sponsor from '@/components/Sponsor.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'Home',
  components: {
    Navbar,
    Category,Kitchen,Sport,Shoes,Client,Sponsor,Footer
  },
  data:()=>({
    toggle:1,
  })
}
</script>
<style scoped>
.v-text-field{font-size:25px;}
.marginLeft{margin-left:-70px;}
.con-mobile{margin-bottom:20rem;margin-top:20rem;}
.mobile{border:4px solid black;}
</style>
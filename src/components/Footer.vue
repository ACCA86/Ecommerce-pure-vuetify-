<template>
    <v-footer dark padless>
        <v-card class="black white--text" width="100%">
            <v-row> 
                <v-col cols="12" sm="12" xs="12" md="6">
                    <v-toolbar flat color="green" height="200%">
                        <v-badge color="rgb(62 126 64)" dot>
                            <v-icon>mdi-cart</v-icon>
                        </v-badge>
                        <v-toolbar-title>
                            <span class="orang--text">e</span><strong>Gerocery</strong>
                        </v-toolbar-title>
                        <v-spacer></v-spacer>
                    <v-row>
                        <v-card-text>
                        <v-btn class="white--text ml-4" icon fab outlined small>
                            <v-icon id="facebook">mdi-facebook</v-icon>
                        </v-btn>
                        <v-btn class="white--text ml-4" icon fab outlined small>
                            <v-icon id="youtube">mdi-youtube</v-icon>
                        </v-btn>
                        <v-btn class="white--text ml-4" icon fab outlined small>
                            <v-icon id="linkedin">mdi-linkedin</v-icon>
                        </v-btn>
                        <v-btn class="white--text ml-4" icon fab outlined small>
                            <v-icon id="twitter">mdi-twitter</v-icon>
                        </v-btn>
                    </v-card-text>
                    </v-row>
                    </v-toolbar>
                </v-col>
                <v-col cols="12" xs="2" sm="2" md="2">
                    <v-card-text class="white--text pt-0 mt-4">
                        <h3>About</h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">How It Work</v-card-text>
                    <v-card-text class="grey--text mt-n4">Our Products</v-card-text>
                    <v-card-text class="grey--text mt-n4">Promotion</v-card-text>
                    <v-card-text class="grey--text mt-n4">Refer a Friend</v-card-text>
                </v-col>
                <v-col cols="12" xs="2" sm="2" md="2">
                    <v-card-text class="white--text pt-0 mt-4">
                        <h3>Delevery</h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">Cost on Delevery</v-card-text>
                    <v-card-text class="grey--text mt-n4">Payment Method</v-card-text>
                    <v-card-text class="grey--text mt-n4">Delevery Astus</v-card-text>
                    <v-card-text class="grey--text mt-n4">Returns</v-card-text>
                </v-col>
                <v-col cols="12" xs="2" sm="2" md="2">
                    <v-card-text class="white--text pt-0 mt-4">
                        <h3>Contact</h3>
                    </v-card-text>
                    <v-card-text class="grey--text mt-n4">Cairo, Egype</v-card-text>
                    <v-card-text class="grey--text mt-n4">Dar El-Salam</v-card-text>
                    <v-card-text class="grey--text mt-n4">www.ibrahim4u.com</v-card-text>
                    <v-card-text class="grey--text mt-n4">+20 l064447786</v-card-text>
                </v-col>
            </v-row>
             <v-card-text class="py-2 white--text text-center gradient mt-n4">
               {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
             </v-card-text>
        </v-card>
    </v-footer>
</template>
<style scoped>
.gradient{
    background-color: #4CAF50;
    background-image:linear-gradient(to right,#419e44,#53a855 ,black);
    }
.v-btn--outlined:nth-child(1):hover{border-color:#1a0dab;}
.v-btn--outlined:nth-child(2):hover{border-color:#f00;}
.v-btn--outlined:nth-child(3):hover{border-color:#0077b5;}
.v-btn--outlined:nth-child(4):hover{border-color:rgb(32, 141, 204);}
.v-btn--outlined:hover #facebook{color:#1a0dab;border-color:#1a0dab;transform: scale(1.2);}
.v-btn--outlined:hover #youtube{border-color:#f00;color:#f00;transform: scale(1.2);}
.v-btn--outlined:hover #linkedin{color:#0077b5;border-color:#0077b5;transform: scale(1.2);}
.v-btn--outlined:hover #twitter{color:rgb(32, 141, 204);border-color:#f00;transform: scale(1.2);}
</style>
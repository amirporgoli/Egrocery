<template>
  <v-footer dark padless>
    <v-card flat tile color="black" class="white--text py-12 px-5" width="100%">
        <v-row>
            <v-col cols="12" xs="12" sm="6" md="4" class="pa-16">
                <v-toolbar color="transparent" flat>
                    <v-badge color="#d5f0db" dot>
                        <v-img src="/src/img/1.png" contain width="30"></v-img>
                    </v-badge>
                    <v-toolbar-title class="ml-4">
                        <span class="green--text">e</span><strong>grocery</strong>
                    </v-toolbar-title>
                </v-toolbar>
                <v-card-text class="pt-0">
                    <v-btn v-for="icon in icons" :key="icon" class="mx-1 white--text" icon fab outlined small>
                        <v-icon size="20">{{ icon }}</v-icon>
                    </v-btn>
                </v-card-text>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="2">
                <v-card-text class="white--text pt-0">
                    About
                </v-card-text>
                <v-card-text class="gray-text">How it Work</v-card-text>
                <v-card-text class="gray-text mt-n4">Our Promrams</v-card-text>
                <v-card-text class="gray-text mt-n4">Promotions</v-card-text>
                <v-card-text class="gray-text mt-n4">Refer A friend</v-card-text>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="2">
                <v-card-text class="white--text pt-0">
                    Delivery
                </v-card-text>
                <v-card-text class="gray-text">Cost on Delivery</v-card-text>
                <v-card-text class="gray-text mt-n4">Payment Method</v-card-text>
                <v-card-text class="gray-text mt-n4">Delivery Astus</v-card-text>
                <v-card-text class="gray-text mt-n4">Returns</v-card-text>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="2">
                <v-card-text class="white--text pt-0">
                    Contact
                </v-card-text>
                <v-card-text class="gray-text">Amir Hoseion Porgoli</v-card-text>
                <v-card-text class="gray-text mt-n4">nor/mazandaran</v-card-text>
                <v-card-text class="gray-text mt-n4">porgoliamir@gmail.com</v-card-text>
                <v-card-text class="gray-text mt-n4">09388125037</v-card-text>
            </v-col>

        </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default {
data() {
    return {
        icons: [
      "/src/img/mdi mdi-apple",
      "/src/img/mdi mdi-google-plus",
      "/src/img/mdi mdi-twitter",
      "/src/img/mdi mdi-facebook",
    ],
 
    }
},
}
</script>

<style>

</style>
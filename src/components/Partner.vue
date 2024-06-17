<template>
  <v-row class="mt-10 px-16">
    <v-col cols="3" v-for="partner in partners" :key="partner">
        <div align="center" justify="center">
            <v-img :src="partner.img" max-height="80" max-width="80" contain></v-img>
        </div>
    </v-col>
  </v-row>
</template>

<script>
export default {
data() {
    return {
        partners: [
      { img: "/src/img/airbnb.png" },
      { img: "/src/img/adidas.png" },
      { img: "/src/img/swords.png" },
      { img: "/src/img/castle.png" },
    ],
    }
},
}
</script>

<style>

</style>
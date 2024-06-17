<template>
  <v-row class="space px-16" justify="center">
    <v-col
      cols="12"
      xs="12"
      sm="6"
      md="4"
      v-for="(product, i) in products"
      :key="i"
    >
      <v-card max-width="300" flat outlined class="mx-auto rounded-xl">
        <div align="center" justify="center">
            <v-img :src="product.img" contain max-width="300" max-height="300"></v-img>
        </div>
        <v-card-title>{{ product.title }}</v-card-title>
        <v-card-title class="text-gray-darken-1 gray--text caption mt-n6">{{ product.subtitle }}</v-card-title>
        <v-card-title class="mt-n4">{{ product.price }}</v-card-title>
        <v-card-actions class="mw-2 mt-n4">
            <v-btn outlined class="add mt-n2">
                <v-icon color="green"  @click="decrement" icon="mdi mdi-minus"></v-icon>
            </v-btn>
            <strong class="mx-2" v-text="bpm"></strong>
            <v-btn outlined class="mt-n2 add">
                <v-icon color="green" @click="increment" icon="mdi mdi-plus"></v-icon>
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn class="mx-2 mt-n3" fab dark small color="green">
                <v-icon dark icon="mdi mdi-shopping"></v-icon>
            </v-btn>
        </v-card-actions>
      </v-card
    ></v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      bpm: 1,
      products: [
        {
          img: "/src/img/pr1.png",
          title: "Cabbage",
          subtitle: "1kg",
          price: "$13",
        },
        {
          img: "/src/img/pr2.png",
          title: "Perry's Ice Cream",
          subtitle: "1kg",
          price: "$23",
        },
        { img: "/src/img/pr3.png", title: "Potato", subtitle: "1kg", price: "$17" },
        {
          img: "/src/img/pr4.png",
          title: "Bundle Pack",
          subtitle: "Potato, Papaya, Oil, Cabbage",
          price: "$40",
        },
        {
          img: "/src/img/pr5.png",
          title: "Oreo Biscuit",
          subtitle: "270GM",
          price: "$20",
        },
        { img: "/src/img/pr6.png", title: "Papaya", subtitle: "1kg", price: "$10" },
      ],
    };
  },
  methods: {
    increment() {
        this.bpm++
    },
    decrement() {
        this.bpm--
    }
  },
};
</script>

<style>
</style>
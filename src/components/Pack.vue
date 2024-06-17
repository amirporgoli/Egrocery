<template>
  <v-row justify="center" class="space px-16 pb-5">
    <v-col cols="12" xs="12" sm="6" md="4" v-for="(Pack,i) in packs" :key="i">
        <v-card class="mx-auto rounded-xl" max-width="300" flat outlined>
            <div align="center" justify="center">
                <v-img :src="Pack.img" max-width="300" max-height="300" contain></v-img>
            </div>
            <v-card-title>{{ Pack.title }}</v-card-title>
        <v-card-title class="text-gray-darken-1 gray--text caption mt-n6">{{ Pack.subtitle }}</v-card-title>
        <v-card-title class="mt-n4">{{ Pack.price }}</v-card-title>
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

        </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
data() {
    return {
        bpm: 1,
        packs: [
      { img: "/src/img/p1.png", title: "Medium Box", subtitle: "Tomato, Cabbage, Oil, Cauliflower", price: "$55" },
      { img: "/src/img/p2.png", title: "Big Pack", subtitle: "Tomato, Cabbage, Oil, Cauliflower", price: "$55" },
      { img: "/src/img/p3.png", title: "Small", subtitle: "Tomato, Cabbage, Oil,Cauliflower ", price: "$55" },
      { img: "/src/img/p4.png", title: "Medium Box", subtitle: "Tomato, Cabbage, Oil,Cauliflower", price: "$55" },
      { img: "/src/img/p5.png", title: "Medium Box", subtitle: "Tomato, Cabbage, Oil,Cauliflower", price: "$55" },
      { img: "/src/img/p6.png", title: "Medium Box", subtitle: "Tomato, Cabbage, Oil,Cauliflower", price: "$55" },
    ],
    }
},
methods: {
    increment() {
        this.bpm++
    },
    decrement() {
        this.bpm--
    }
  },
}
</script>

<style>

</style>
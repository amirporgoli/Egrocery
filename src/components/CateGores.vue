<template>
  <v-item-group>
    <v-container>
      <v-row justify="center" class="space">
        <v-col
          cols="12"
          xs="12"
          sm="4"
          md="2"
          v-for="(category, i) in categories"
          :key="i"
        >
          <v-item v-slot="{ active, toggle }">
            <v-card
              :color="active ? '#d5f0db' : 'white'"
              :class="active ? 'borderme' : 'borderout'"
              class="d-flex rounded-lg mx-2 align-center"
              dark height="180" flat @click="toggle"
            >
        <v-row>
            <v-col cols="12" sm="12">
                <v-list-item three-line class="text-center">
                    <v-list-item-content>
                        <div align="center" justify="center">
                            <v-img max-height="80" max-width="80" contain :src="category.img"></v-img>
                        </div>
                        <v-list-item-subtitle :class="active ? 'green--text' : 'black--text'"
                        class="caption mt-4">
                            {{ category.title }}
                        </v-list-item-subtitle>
                    </v-list-item-content>
                </v-list-item>
            </v-col>
        </v-row></v-card>
          </v-item>
        </v-col>
      </v-row>
    </v-container>
  </v-item-group>
</template>

<script>
export default {
  data() {
    return {
      categories: [
        { img: "/src/img/01.png", title: "Meat & Fish" },
        { img: "/src/img/02.png", title: "Vegetables" },
        { img: "/src/img/3.png", title: "Medicine" },
        { img: "/src/img/4.png", title: "Baby" },
        { img: "/src/img/5.png", title: "Office" },
        { img: "/src/img/6.png", title: "Beauty" },
      ],
    };
  },
};
</script>

<style>
</style>
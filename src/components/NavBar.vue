<template>
  <v-app-bar app color="white" flat>
    <v-badge dot floating color="#D5F0DB">
        <v-img src="/src/img/1.png" contain width="30"></v-img>
    </v-badge>
    <v-toolbar-title class="ml-4">
        <span color="#81C784">e</span><strong>Grocery</strong>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-badge color="#FF6D59" content="2" overlap class="mr-2 mt-1">
        <v-avatar color="#FFF0EE" size="40">
            <v-icon size="x-small" color="#FF6D59" icon="mdi mdi-heart"></v-icon>
        </v-avatar>
    </v-badge>
    <v-badge color="#41ab55" content="3" overlap class="mr-2 mt-1">
        <v-avatar color="#ecf7ee" size="40">
            <v-icon size="x-small" color="#41ab55" icon="mdi mdi-shopping"></v-icon>
        </v-avatar>
    </v-badge>
    <span class="gray--text d-none d-sm-flex">Hello<strong>Amir</strong></span>
    <v-avatar size="30" class="ml-2">
        <v-img src="https://cdn.vuetifyjs.com/images/lists/2.jpg"></v-img>
    </v-avatar>
    <v-btn icon dark>
        <v-icon size="x-small" color="#878a94" icon="mdi mdi-chevron-down"></v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {

}
</script>

<style>
.v-toolbar__title {
    font-size: 1rem !important;
}
</style>
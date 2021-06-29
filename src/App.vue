<template>
  <v-app>
    <v-app-bar
      color="white"
      dark
      class="px-16"
    >
      <v-img class="mx-2" src='./assets/logo.svg' max-height="48" max-width="137"></v-img>
      <v-spacer></v-spacer>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">HOME</v-btn></v-toolbar-title>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">ABOUT</v-btn></v-toolbar-title>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">PROGRAMS</v-btn></v-toolbar-title>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">EVENTS</v-btn></v-toolbar-title>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">SCHOOLS</v-btn></v-toolbar-title>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">JOBS</v-btn></v-toolbar-title>
      <v-toolbar-title class='mx-4'><v-btn text color="#606060">CONTACT US</v-btn></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
      text
      color="#606060"
      class="text-capitalize"
      >
        <v-icon left >
          mdi-account-circle
        </v-icon>
        Member
      </v-btn>   
    </v-app-bar>
    
    <v-main>
      <!-- <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" max-height="800"></v-parallax> -->
      <v-parallax
        height="866"
        src="./assets/hero.png"
      >
        <v-row
          align="top"
          justify="center"
        >
          <v-col
            class="text-center"
            cols="12"
          >
            <h1 class="text-h1 font-weight-bold text--primary mt-16">
              6800+ Alumni
            </h1>
            <h4 class="text-h3 text--primary mt-6">
              Build your network all over the world today!
            </h4>
            
            <v-btn
              class="mt-10"
              color="#EB5E5E"
              elevation="2"
              dark
            >Read More</v-btn>
          </v-col>
        </v-row>
      </v-parallax>
      <v-layout
        class="d-flex justify-center mb-6"
        :color="$vuetify.theme.dark ? 'grey darken-3' : 'grey lighten-4'"
        flat
        tile
      >
        <v-flex
          v-for="n in 10"
          :key="n"
          class="pa-2"
          outlined
          tile
        >
          LOGO
        </v-flex>
      </v-layout>

      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style>
/* ini sementara */
  @import url('https://fonts.googleapis.com/css?family=Quicksand');

html, body, {
  font-family: 'Quicksand';
}

#app {
  font-family: 'Quicksand';
}
</style>

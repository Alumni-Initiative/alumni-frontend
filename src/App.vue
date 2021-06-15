<template>
  <v-app>
    <v-app-bar
      color="white"
      dark
    >
      <!-- <v-app-bar-nav-icon>X</v-app-bar-nav-icon> -->
      <v-img height="48" width="137" src='./assets/logo.svg'></v-img>
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

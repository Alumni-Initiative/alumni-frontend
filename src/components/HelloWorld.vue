<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <!-- <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        /> -->
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Router view -> views home > HelloWork.vue
        </h1>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <!-- <h2 class="headline font-weight-bold mb-3">
          What's next?
        </h2> -->

        <v-row justify="center">
          <a
            v-for="(next, i) in whatsNext"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>
        </v-row>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <!-- <h2 class="headline font-weight-bold mb-3">
          Important Links
        </h2> -->

        <v-row justify="center">
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ link.text }}
          </a>
        </v-row>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <!-- <h2 class="headline font-weight-bold mb-3">
          Ecosystem
        </h2> -->

        <v-row justify="center">
          <a
            v-for="(eco, i) in ecosystem"
            :key="i"
            :href="eco.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ eco.text }}
          </a>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      ecosystem: [
        {
          text: 'text1',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'text2',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'text3',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'text4',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'text5',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'text6',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'text7',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'text8',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'text9',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'text10',
          href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
        },
        {
          text: 'text11',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>

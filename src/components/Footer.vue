<template>
  <v-container>
    <v-footer color="black" padless>
      <v-col class="text-center" cols="12">
        <v-card color="black" flat tile class="white--text text-center">
          <v-card-text>
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4 white--text"
              icon
            >
              <a :href="icon.link"
                ><v-icon light size="24px">
                  {{ icon.icon }}
                </v-icon></a
              >
            </v-btn>
          </v-card-text>

          <v-divider></v-divider>

          <v-card-text class="white--text">
            {{ new Date().getFullYear() }} — <strong>Brandon Cortes</strong>
          </v-card-text>
        </v-card>
      </v-col>
    </v-footer>
  </v-container>
</template>

<script>
export default {
  name: "Footer",

  data: () => ({
    icons: [
      {
        icon: "mdi-facebook",
        link: "https://www.facebook.com/brandoneduardo.cortescorrea/",
      },
      {
        icon: "mdi-twitter",
        link: "https://twitter.com/B2OriginalTM",
      },
      {
        icon: "mdi-gmail",
        link: "brandon.cortes.1690@gmail.com",
      },
    ],
  }),
};
</script>
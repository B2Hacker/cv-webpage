<template>
  <v-app>
    <v-app-bar app flat color="purple">
      <NavBar />
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>

    <v-footer flat >
      <Footer />
    </v-footer>
  </v-app>
</template>

<script>
import Footer from "./components/Footer.vue";
import NavBar from "./components/NavBar.vue";

export default {
  name: "App",

  components: {
    Footer,
    NavBar,
  },

  data: () => ({
    //
  }),
};
</script>

<template>
  <v-app>
    <v-app-bar
      app
      color="purple"
      dark
    >
      <div class="d-flex align-center">
      <i class="fab fa-black-tie fa-3x"></i></div>
      <div><v-btn to="/" plain><v-toolbar-title>Brandon Cortes</v-toolbar-title></v-btn>
      </div>
      <v-btn to="/Certification" plain>Certification</v-btn>

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

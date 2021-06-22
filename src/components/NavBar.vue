<template>
  <v-container>
    <v-toolbar flat color="purple">
      <i class="fab fa-black-tie fa-3x"></i>
      <v-btn to="/" plain>
        <v-toolbar-title>Brandon Cortes</v-toolbar-title>
      </v-btn>
      
      <v-toolbar-items>
        <v-btn to="/SkillsandInterest" plain>Skills And Interests</v-btn>
        <v-btn to="/Certification" plain>Certifications</v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </v-container>
</template>

<script>
export default {
  name: "NavBar",

  data: () => ({}),
};
</script>
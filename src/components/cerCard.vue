<template>
  <div class="block cerCardBlock">
    <v-container>
      <h2 class="text-center">Certifications</h2>
      <v-row>
        <v-col cols="4" v-for="item in items" :key="item.id">
          <v-card outlined class="mx-auto">
            <v-card-title>{{item.title}}</v-card-title>
            <v-img
              max-height="auto"
              max-width="auto"
              :src="item.src"
            >
              
            </v-img>

            <v-card-subtitle class="pb-0"> {{item.subtitle}} </v-card-subtitle>

            <v-card-text class="text--primary">
              <div>{{item.description}}</div>
            </v-card-text>

            <v-card-actions>
              <v-btn color="primary" text> WIP </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "cerCard",
  data: () => ({
    show: false,
    items: [
            {
        id: 1,
        title: "TSU Certificate",
        subtitle: "Diciembre 2020",
        description: "His ubique laboramus ne. Expetenda assueverit sed ad. Id nec malis lucilius delicatissimi. Nec assum sonet suscipit ex, diam deterruisset ut usu, ad dicat fabellas aliquando eam.",
        src: require("../assets/certificates/img003.jpg")
      },
      {
        id: 2,
        title: "ITEP Certificate",
        subtitle: "1,000 miles of wonder",
        description: "His ubique laboramus ne. Expetenda assueverit sed ad. Id nec malis lucilius delicatissimi. Nec assum sonet suscipit ex, diam deterruisset ut usu, ad dicat fabellas aliquando eam.",
        src: require("../assets/certificates/img002.jpg")
      },
                  {
        id: 3,
        title: "Duolingo Certificate",
        subtitle: "1,000 miles of wonder",
        description: "His ubique laboramus ne. Expetenda assueverit sed ad. Id nec malis lucilius delicatissimi. Nec assum sonet suscipit ex, diam deterruisset ut usu, ad dicat fabellas aliquando eam.",
        src: require("../assets/certificates/img001.jpg")
      },
                  {
        id: 4,
        title: "Nuevo Ladero City College Certificate",
        subtitle: "1,000 miles of wonder",
        description: "His ubique laboramus ne. Expetenda assueverit sed ad. Id nec malis lucilius delicatissimi. Nec assum sonet suscipit ex, diam deterruisset ut usu, ad dicat fabellas aliquando eam.",
        src: require("../assets/certificates/NLCC.png")
      },
                  {
        id: 5,
        title: "MUNUT Certificate",
        subtitle: "1,000 miles of wonder",
        description: "His ubique laboramus ne. Expetenda assueverit sed ad. Id nec malis lucilius delicatissimi. Nec assum sonet suscipit ex, diam deterruisset ut usu, ad dicat fabellas aliquando eam.",
        src: require("../assets/certificates/img004.jpg")
      },
                  {
        id: 6,
        title: "Cisco CyberSecurity Certificate",
        subtitle: "1,000 miles of wonder",
        description: "His ubique laboramus ne. Expetenda assueverit sed ad. Id nec malis lucilius delicatissimi. Nec assum sonet suscipit ex, diam deterruisset ut usu, ad dicat fabellas aliquando eam.",
        src: require("../assets/certificates/Cisco.png")
      },
    ],
  }),
};
</script>
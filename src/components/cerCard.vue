<template>
  <div class="block cerCardBlock">
    <v-container>
      <br>
      <h2 class="text-center">Certifications</h2>
      <br>
      <br>
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
              <div>{{item.institution}}</div>
              <div>{{item.description}}</div>
            </v-card-text>
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
        subtitle: "December 2020",
        institution: "Institution: Universidad Tecnologica de Tamaulipas Nortes (UTTN)",
        description: "The Higher University Technician in Information Technologies in the area of Virtual Environments and Digital Business has the necessary professional competencies to perform in the labor field, locally, regionally and nationally.",
        src: require("../assets/certificates/img003.jpg")
      },
      {
        id: 2,
        title: "ITEP Certificate",
        subtitle: "04/11/2019",
        institution: "Institution: International Test of English Proficiency (iTEP)",
        description: "Can understand a wide range of demanding, longer texts, and recognize implicit meaning.Can express him/herself fluently and spontaneously without much obvious searching forexpressions.",
        src: require("../assets/certificates/img002.jpg")
      },
                  {
        id: 3,
        title: "Duolingo Certificate",
        subtitle: "12/12/2020",
        institution: "Plataform: Duolingo Eglish Test",
        description: "Can understand a variety of demanding written and spoken language including some specialized language use situations. Can grasp implicit, figurative, pragmatic, and idiomatic language.",
        src: require("../assets/certificates/img001.jpg")
      },
                  {
        id: 4,
        title: "Nuevo Ladero City College Certificate",
        subtitle: "01/22/2011 - 04/15/2017",
        institution: "Institution: Nuevo Laredo City College",
        description: "Over the past fifty years, English has been considered the premier international language. Learning and mastering English has become a primary skill in demand in both academic and workplace settings.",
        src: require("../assets/certificates/NLCC.png")
      },
                  {
        id: 5,
        title: "MUNUT Certificate",
        subtitle: "10/22/2019",
        institution: "Institution: Universidad Teclologica de Nuevo Laredo (UTNL)",
        description: "The Model United Nations is a simulation of the sessions of this organization, where the participating delegations are divided into committees, which during their meetings will have the opportunity to propose actions to solve global problems, such as human rights, climate change, international security and economy, among others.",
        src: require("../assets/certificates/img004.jpg")
      },
                  {
        id: 6,
        title: "Cisco CyberSecurity Certificate",
        subtitle: "04/13/2021",
        institution: "Plataform: Cisco Networking Academy",
        description: "Cisco Networking Academy transforms the lives of learners, educators and communities through the power of technology, education and career opportunities. Available to anyone, anywhere.",
        src: require("../assets/certificates/Cisco.png")
      },
    ],
  }),
};
</script>
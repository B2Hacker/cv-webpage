<template>
  <div class="about" align-center>
    <v-container>
      <br />
      <br />
      <v-card>
        <ul>
          <v-col cols="12">
            <br />
            <h2 class="text-center headline font-weight-bold mb-3">
              <FONT FACE="Tahoma">Skills</FONT>
            </h2>
            <br />
            <v-col cols="12">
              <v-img
                :src="require('../assets/skills.png')"
                class="my-3"
                contain
                height="200"
              />
            </v-col>
            <br />
            <br />
          </v-col>
        </ul>
      </v-card>
      <br />
      <br />
      <v-card>
        <ul>
          <v-col cols="12">
            <br />
            <h2 class="text-center headline font-weight-bold mb-3">
              <FONT FACE="Tahoma">Interests</FONT>
            </h2>
            <br />
            <h3>
              <FONT FACE="Arial">
                I would like to be able to develop in the area of systems and
                put into practice my knowledge of web andmobile application
                programming, database development in a work situation. Also to
                be able to enrich myknowledge of Mechatronics in the work areas
                where electronics and mechanics are involved.
              </FONT>
            </h3>
            <br />
            <br />
          </v-col>
        </ul>
      </v-card>
      <br />
      <br />
      <v-card>
        <ul>
          <v-col cols="12">
            <h2 class="text-center headline font-weight-bold mb-3">
              <FONT FACE="Tahoma">Languages</FONT>
            </h2>
            <br />
            <h3 text align class="headline font-weight-bold mb-3">
              English (Advance)
            </h3>
            <h3>
              <FONT FACE="Tahoma">
                Can understand a wide range of demanding, longer texts, and
                recognize implicit meaning.Can express him/herself fluently and
                spontaneously without much obvious searching forexpressions.
              </FONT>
            </h3>
            <h3>
              <FONT FACE="Tahoma">
                Can understand a variety of demanding written and spoken
                language including some specialized language use situations. Can
                grasp implicit, figurative, pragmatic, and idiomatic language.
              </FONT>
            </h3>
            <br />
            <h3>
              <li>ITEP: C1</li>
              <li>Duolingo Exam: 125</li>
              <li>NLCC: 6 years of english classes.</li>
            </h3>
            <br />
          </v-col>
        </ul>
      </v-card>
      <br />
      <br />
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Skills",

  data: () => ({}),
};
</script>
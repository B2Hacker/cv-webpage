<template>
  <div class="about" align-center>
    <v-container>
      <v-row class="text-center">
        <v-col cols="12">
          <v-img
            align-center
            :src="require('../assets/BC.jpeg')"
            class="my-3"
            contain
            height="200"
          />
        </v-col>

        <v-col class="mb-4">
          <h1 text align class="display-2 font-weight-bold mb-3">
            <FONT FACE="Courier"> Brandon Eduardo Cortes Correa</FONT>
          </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-card>
      <ul>
        <h1 text align class="display-2 font-weight-bold mb-3">
          <FONT FACE="Tahoma"><li>Personal Information:</li></FONT>
        </h1>
        <v-col cols="12">
          <h3>
            <p>
              Address: Sierra Nevada #619, Las Fuentes Sección Lomas, C.P.88703
              Reynosa, Tamps.
            </p>
            <p>Cell: 8994934346 Tel:8999510288</p>
            <p>Email: brandon.cortes.1690@gmail.com</p>
          </h3>
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
            <FONT FACE="Tahoma">About me</FONT>
          </h2>
          <br />
          <h3>
            <FONT FACE="Arial">
              Experience in web development and administrative area. Knowledge
              of Office and various software development tools such as visual
              code or studio. Knowledge in languages such as C#, HTML and
              JavaScript. He has worked as a Web Developer in the creation of
              pages for some companies and as an Administrative Assistant in the
              IMSS performing administrative functions. Positive and
              perseverant, I do not let myself be defeated by obstacles or
              challenges. Good at working in a team and socializing with others.
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
            <FONT FACE="Tahoma">Experience</FONT>
          </h2>
          <br />
          <h3 text align class="headline font-weight-bold mb-3">
            IMSS 2017 - 2018
          </h3>
          <h3>
            <FONT FACE="Tahoma">
              Administrative Assistant in charge of guarding and receiving
              official documents, interacting with the public, processing files,
              communicating with the department, making photocopies and
              processing information through a database. Developed communication
              skills and built organizational capacity.
            </FONT>
          </h3>
          <br />
          <h3>
            <li>File, organize, store and review all types of documents.</li>
            <li>Record information by updating databases or computer files.</li>
            <li>Maintain a clean and orderly work area.</li>
          </h3>
          <br />
          <br />
          <h3 text align class="headline font-weight-bold mb-3">
            Cibercafé Neo 2018 - 2019
          </h3>
          <h3>
            <FONT FACE="Tahoma">
              Junior web developer in charge of making an advertising website
              that includes a database for the inventory of an Internet cafe,
              this was developed with C # in the visual studio program with
              clean and efficient code based on customer specifications. It was
              possible to implement the computer skills acquired with the
              studies and to develop these with new knowledge.
            </FONT>
          </h3>
          <br />
          <h3>
            <li>Creation of advertising banners to promote the store.</li>
            <li>Creation of a database to store the store inventory.</li>
            <li>Creation of a web page for users and employees.</li>
          </h3>
          <br />
          <br />
          <h3 text align class="headline font-weight-bold mb-3">
            Vivendo 2020 - 2021
          </h3>
          <h3>
            <FONT FACE="Tahoma">
              Junior web developer in charge of building a website for a
              Canadian client of Vivendo. This page stores client's information
              in a database that the client can edit himself. This was done with
              visual code with a framework called NextJS. I was able to learn to
              work with people from abroad and develop myself in new programming
              languages not seen before.
            </FONT>
          </h3>
          <br />
          <h3>
            <li>Creation of database to store client's information.</li>
            <li>
              Creation of editable web page according to client's
              specifications.
            </li>
            <li>
              Worked with a person from abroad, developing bilingual skills.
            </li>
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
            <FONT FACE="Tahoma">Education</FONT>
          </h2>
          <br>
          <v-row>
            <v-col cols="6" v-for="item in items" :key="item.id">
              <v-card outlined class="mx-auto">
                <v-card-title>{{ item.title }}</v-card-title>
                <v-img max-height="auto" max-width="auto" :src="item.src">
                </v-img>

                <v-card-subtitle class="pb-0">
                  {{ item.subtitle }}
                </v-card-subtitle>

                <v-card-text class="text--primary">
                  <div>{{ item.institution }}</div>
                  <div>{{ item.description }}</div>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </v-col>
      </ul>
    </v-card>
    <br />
    <br />
  </div>
</template>

<script>
export default {
  name: "CV",

  data: () => ({
    items: [
            {
        id: 1,
        title: "Universidad Tecnologica de Tamaulipas Norte (UTTN)",
        subtitle: "2018 – 2020",
        institution: "Higher University Technician in Information Technology",
        description: "Develop technological solutions for Web environments using object-oriented programming, database and local area network fundamentals that meet the needs of organizations. Implement multiplatform, cloud and embedded software solutions in secure environments through data acquisition and management and software engineering to contribute to the automation of processes in organizations.",
        src: require("../assets/UTTNlogo.png")
      },
      {
        id: 2,
        title: "Centro de Bachillerato Tecnologico Industrial y de Servicios No.7 (CBTIS No.7)",
        subtitle: "2015 – 2018",
        institution: "Mechatronics Technician",
        description: "Perform diagnosis, installation, reconversion and maintenance tasks to mechatronic systems, detect anomalies in automated production processes and perform corrective and preventive maintenance in integral processes, verifying the operation of sensors, actuators, mechanisms and computer programs that govern production.",
        src: require("../assets/cbtis7logo2.png")
      },
    ],
  }),
};
</script>

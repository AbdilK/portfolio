<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Projects</h2>
      <v-row>
        <v-col cols="4" v-for="item in items" :key="item.id">
          <v-card
            outlined
            class="mx-auto"
            max-width="400"
            color="#212121"
            margin-top="20px"
          >
            <v-img class="white--text align-end" height="200px" :src="item.src">
              <v-card-title> {{ item.title }} </v-card-title>
            </v-img>

            <v-card-subtitle class="grey--text pb-0">
              {{ item.subtitle }}
            </v-card-subtitle>

            <v-card-text class="white--text">
              <div>{{ item.description }}</div>
            </v-card-text>

            <v-card-actions v-show="item.readMoreUrl !== ''">
              <v-btn color="amber" text :href="item.readMoreUrl" target="_blank"
                >Læs mere</v-btn
              >
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "myProjects",

  data() {
    return {
      items: [
        {
          id: 1,
          title: "1. Semester eksamensprojekt",
          subtitle: "Donations website omkring plastforurening",
          description:
            "I forbindelse med første semester eksamen, udviklede jeg en hjemmeside baseret på ren HTML, CSS og JS. Hjemmeside er en informations side, hvor der er mulighed for at lave en donation.",
          src: require("../assets/images/oceanEye.png"),
          readMoreUrl: "http://www.akoycu.dk",
        },

        {
          id: 2,
          title: "1. Semester eksamensprojekt",
          subtitle: "Designmanual rapport",
          description:
            "Ved siden af informations siden til første semester eksamen, skulle vi aflevere en rapport samt designmanual. Rapporten blev rigtig pæn, med et innovativt design. ",
          src: require("../assets/images/designManual.jpg"),
          readMoreUrl: "../images/designManual.jpg",
        },
        {
          id: 3,
          title: "Timeline Museum Logo contest",
          subtitle: "1# Konkurrence om bedste logo",
          description:
            "På andet semester, fik vi en opgave, hvor vi skulle designe et logo til en mobilapplikation. Denne app skulle være til et museum, hvor folk kan læse om historiske begivenheder, baseret på en tidslinje. Mit design vandt konkurrencen",
          src: require("../assets/images/LogoContest.png"),
          readMoreUrl: "hej",
        },
        {
          id: 4,
          title: "20 movies not to miss in 2020",
          subtitle: "3,000 miles of wonder",
          description:
            "Aliquam albucius mei ei, debitis torquatos et pro, eos natum scribentur no. Putant verear constituto te qui. Adolescens persequeris vim ei. Vel nullam reprimique te.",
          src: require("../assets/images/placeholder.png"),
          readMoreUrl: "hej",
        },
        {
          id: 5,
          title: "20 movies not to miss in 2020",
          subtitle: "3,000 miles of wonder",
          description:
            "Aliquam albucius mei ei, debitis torquatos et pro, eos natum scribentur no. Putant verear constituto te qui. Adolescens persequeris vim ei. Vel nullam reprimique te.",
          src: require("../assets/images/placeholder.png"),
          readMoreUrl: "hej",
        },
        {
          id: 6,
          title: "20 movies not to miss in 2020",
          subtitle: "3,000 miles of wonder",
          description:
            "Aliquam albucius mei ei, debitis torquatos et pro, eos natum scribentur no. Putant verear constituto te qui. Adolescens persequeris vim ei. Vel nullam reprimique te.",
          src: require("../assets/images/placeholder.png"),
          readMoreUrl: "hej",
        },
      ],
    };
  },
};
</script>

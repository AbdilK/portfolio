<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Projects</h2>
      <h3 class="text-center" >Vil du gerne se mere af mine projekter?<br> 
      Jeg har samlet nogle af de bedste projekter, som jeg har arbejdet på under uddannelsen. 
      <br>
      Alt fra hjemmesider og logo design processer til video & kortfilm produktion.</h3>
      <br>
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
          title: "No way out",
          subtitle: "8 minutters kortfilm",
          description:
            "På tredje semester skulle vi lave en kortfilm, hvor vi skulle benytte os af alle de ting vi har lært i AV - Productions faget. Kortfilmen blev til en gyser/thriller på 8 minutter.",
          src: require("../assets/images/kortfilm.png"),
          readMoreUrl: "https://www.youtube.com/watch?v=JEt7sPA1r4M",
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
          title: "Sixth Car Rental",
          subtitle: "XD Prototype",
          description:
            "XD Prototype af en biludlejningshjemmeside, som er fuldt funktionel med sidehenvisninger som fx. når man surfer rundt på siden.",
          src: require("../assets/images/rentalcars.png"),
          readMoreUrl: "",
        },
        {
          id: 5,
          title: "1. Semester eksamensprojekt",
          subtitle: "Designmanual rapport",
          description:
            "Ved siden af informations siden til første semester eksamen, skulle vi aflevere en rapport samt designmanual. Rapporten blev rigtig pæn, med et innovativt design. ",
          src: require("../assets/images/designManual.jpg"),
          readMoreUrl: "",
        },
        {
          id: 6,
          title: "OceanEye Logo Design",
          subtitle: "Designprocessen",
          description:
            "Ved udarbejdelsen af logo'et til vores første semester projekt, har vi været igennem en lang process. På billedet ses processen, hvilke overvejser vi har haft. Det endelige logo er symmetrisk hele vejen rundt. ",
          src: require("../assets/images/logodesignprocess.png"),
          readMoreUrl: "",
        },
      ],
    };
  },
};
</script>

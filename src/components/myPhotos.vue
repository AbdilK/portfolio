<template>
  <div class="section myPhotos">
    <v-container>
      <h2 class="text-center" amber accent-3>Billede redigering</h2>
      <h3 class="text-center">
        Jeg ELSKER at tage flotte billeder af skulpturer, landskaber og bygninger.<br />
        Her er et par eksempler på nogle bileder, som der er leget med, som fx. kontrasten, lysforholdende, vejr ændringer og
        tilføjelser på græsset.
      </h3>
      <v-row>
        <v-col
          v-for="item in items"
          :key="item.id"
          class="d-flex child-flex"
          cols="6"
          sm="4"
        >
          <v-card flat tile class="d-flex">
            <v-img :src="item.src" aspect-ratio="1" class="grey lighten-2">
              <template v-slot:placeholder>
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-progress-circular
                    indeterminate
                    color="grey lighten-5"
                  ></v-progress-circular>
                </v-row>
              </template>
            </v-img>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "myPhotos",
  data() {
    return {
      items: [
        {
          id: 1,
          src: require("../assets/images/hjul.png"),
        },
        {
          id: 2,
          src: require("../assets/images/3mænd.png"),
        },
        {
          id: 3,
          src: require("../assets/images/mænd.png"),
        },
        {
          id: 4,
          src: require("../assets/images/denmarkedit.jpg"),
        },
        {
          id: 5,
          src: require("../assets/images/fogedit.jpg"),
        },
        {
          id: 6,
          src: require("../assets/images/bridgeedit.jpg"),
        },
      ],
    };
  },
};
</script>
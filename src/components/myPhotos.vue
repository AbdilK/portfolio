<template>
  <div class="block galleryBlock">
    <v-container >
      <h2 class="text-center" amber accent-3>Photoshoot</h2>
      <h3 class="text-center" >Seneste photoshoot af Strandvejen i Hjerting. <br> 
      Taget i forbindelse med et skoleprojekt, og som efterfølgende er blevet redigeret i Photoshop.
      <br>
      Der er leget med kontrasten, lysforholdende, vejr ændringer og tilføjelser på græsset.</h3>
      <v-row>
        <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="6" sm="4">
          <v-card flat tile class="d-flex">
            <v-img :src="item.src" aspect-ratio="1" class="grey lighten-2">
              <template v-slot:placeholder>
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
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
          src: require("../assets/images/hjul.png")
        },
        {
          id: 2,
          src: require("../assets/images/3mænd.png")
        },
        {
          id: 3,
          src: require("../assets/images/mænd.png")
        }
      ]
    };
  }
};
</script>
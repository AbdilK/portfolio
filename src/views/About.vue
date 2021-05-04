<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/img13.jpg">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <div class="headline">About</div>
            </v-container>
          </v-col>
        </v-row>
      </v-img>
    </div>
    <div class="block">
      <v-container>
        <p>
          Mit navn er Abdil Koycu. Jeg er 25 år gammel og bor i Oksbøl. Til dagligt læser jeg til Multimediedesigner på Erhvervsakademiet SydVest. Nedenstående er en video af mit CV. 
        </p>
        <div class="your-centered-div">
          <youtube
            :video-id="videoId"
            ref="youtube"
            @playing="playing"
            float="center"
          ></youtube>
        </div>
      </v-container>
    </div>
    <div class="block">
      <v-container>
        <h2 class="text-center">Abdil Köycü</h2>
        <v-row>
          <v-col v-for="item in items" :key="item.id" class="d-flex child-flex">
            <v-card flat tile class="mx-auto">
              <v-img
                :src="item.src"
                aspect-ratio="1"
                class="grey lighten-2"
              ></v-img>
              <v-card-text class="text--primary text-center">
                <div class="title">{{ item.name }}</div>
                <h4>{{ item.title }}</h4>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </v-content>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      videoId: "WP3G9NPXmNM",
      items: [
        {
          id: 1,
          src: require("../assets/images/me2.png"),
          name: "Abdil Koycu",
          title: "Multimediedesigner",
        },
      ],
    };
  },
};
</script>
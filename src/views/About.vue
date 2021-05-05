<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/img13.jpg" >
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
        <h2 class="text-center">Abdil Köycü</h2>
        <v-row>
          <v-col v-for="item in items" :key="item.id" class="d-flex child-flex " cols="12" sm="4" >
            <v-card flat tile class="mx-auto amber accent-3"  >
              <v-img
                :src="item.src"
                aspect-ratio="1"
                class="grey lighten-2"
                
              ></v-img>
              <v-card-text class="text--primary text-center ">
                <div class="title">{{ item.name }}</div>
                <h4>{{ item.title }}</h4>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="block">
      <v-container class="text-center">
        <p>
          Mit navn er Abdil Koycu. Jeg er 25 år gammel og bor i Oksbøl. <br> Til dagligt læser jeg til Multimediedesigner på Erhvervsakademiet SydVest.
          <br> Se mere i videoen herunder:
        </p>
        <div class="text-center">
          <youtube
            :video-id="videoId"
            ref="youtube"
            @playing="playing"
            float="center"
          ></youtube>
          
        </div>
      
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
          src: require("../assets/images/BusinessCard.png"),
          name: "Business Kort Design",
          title: "Klik her for at downloade",
        },
        {
          id: 1,
          src: require("../assets/images/abdilme.png"),
          name: "Abdil Koycu",
          title: "Multimediedesigner",
        },
        {
          id: 1,
          src: require("../assets/images/CV.png"),
          name: "Curriculum Vitae (CV)",
          title: "Klik her for at downloade",
        },
      ],
    };
  },
};
</script>
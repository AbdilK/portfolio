<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/aboutme.png" >
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <div class="headline"></div>
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
                <a :href="item.URLLink">
                <h4>{{ item.title }}</h4></a>  
              </v-card-text>

            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="block">
      <v-container class="text-center">
        <h2 class="text-center" >Curriculum Vitae Video</h2>
        <h3>
          Mit navn er Abdil Koycu. Jeg er 25 år gammel og bor i Oksbøl. <br> Til dagligt læser jeg til Multimediedesigner på Erhvervsakademiet SydVest.
          <br> Se mere i videoen herunder:
          
          <br>
        </h3>
        <div cols="12" md="4" class="text-center">
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
          URLLink: "../assets/images/BusinessCard.png"
        },
        {
          id: 1,
          src: require("../assets/images/abdilme.png"),
          name: "Abdil Koycu",
          titles: "Multimediedesigner",
        },
        {
          id: 1,
          src: require("../assets/images/CV.png"),
          name: "Curriculum Vitae (CV)",
          title: "Klik her for at downloade",
          URLLink: "../assets/images/AbdilCV.pdf"
        },
      ],
      contacts: [
        {
          id: 1,
          
          name: "ADDRESSE",
          title: "Spangsbjerg Kirkevej 103, 6700 Esbjerg",
          readMoreUrl: "https://www.google.com/maps/place/Erhvervsakademi+SydVest/@55.4877012,8.4469108,15z/data=!4m2!3m1!1s0x0:0xf131cc5b28fe1f27?sa=X&amp;ved=2ahUKEwjA4urJps3tAhXlo4sKHdEbCZYQ_BIwDXoECBsQBQ"
        },
        {
          id: 2,
          name: "TELEFON",
          title: "+45 42 22 76 XX",
          readMoreUrl: "tel:+4542227612"
        },
        {
          id: 3,
         
          name: "MAIL",
          title: "ak@akoycu.dk",
          readMoreUrl: "mailto:AK@akoycu.dk"
        },
      ],
    };
  },
};
</script>
<template>
  <v-content>
    <div class="static contact">
      <v-img src="../assets/images/contact.png">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
        </v-row>
      </v-img>
    </div>
    <div class="section">
      <div class="section">
        <v-container>
          <h2 class="text-center">Kontakt</h2>
          <h3 class="text-center">
            Synes du, at mit arbejde ser spændende ud, og har du brug for en ung
            frisk gut som mig? <br />
            Tøv ikke, kontakt mig endelig for, at få et uforpligtende tilbud!
            <br />
            Ring på nedenstående telefon nummer, eller smid mig en besked over
            mail. <br /><br />
            Ser frem til at høre fra dig!
            <br />
            <br />
          </h3>
          <v-row>
            <v-col
              v-for="contacts in contacts"
              :key="contacts.id"
              class="d-flex child-flex"
              cols="12"
              sm="4"
            >
              <v-card flat tile class="mx-auto amber accent-3">
                <v-card-text class="text--primary text-center">
                  <div class="title">{{ contacts.name }}</div>
                  <h4>{{ contacts.title }}</h4>
                  <h4>{{ contacts.titles }}</h4>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </div>
    </div>
    <div class="googlemap">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2260.563738484516!2d8.44472211592027!3d55.48770118048331!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x464b20de0dc1b019%3A0xf131cc5b28fe1f27!2sErhvervsakademi%20SydVest!5e0!3m2!1sda!2sdk!4v1620216100927!5m2!1sda!2sdk"
        width="100%"
        height="450"
      ></iframe>
    </div>
  </v-content>
</template>

<script>
export default {
  name: "Contact",
  data: () => ({
    contacts: [
      {
        id: 1,

        name: "ADDRESSE",
        title: "Spangsbjerg Kirkevej 103, 6700 Esbjerg",
      },
      {
        id: 2,
        name: "TELEFON",
        title: "+45 42 22 76 12",
      },
      {
        id: 3,

        name: "E-MAIL",
        title: "ak@akoycu.dk",
      },
    ],
  }),
};
</script>
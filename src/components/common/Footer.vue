<template>
  <v-container>
    <v-footer dark padless>
      <v-card flat tile class="grey darken-4 white--text text-center">
        <v-card-text>
          <v-btn
            v-for="icon in icons"
            :key="icon"
            class="mx-4 white--text"
            icon
          >
            <v-icon size="24px">
              {{ icon }}
            </v-icon>
          </v-btn>
        </v-card-text>

      

        <v-divider></v-divider>

        <v-card-text class="white--text">
         © {{ new Date().getFullYear() }} — Alle rettigheder forbeholdes. Kopiering fra elementer og opgaver må kun finde sted på institutioner eller virksomheder, der har indgået aftale med <strong>ABDIL KÖYCÜ</strong>, og kun inden for de rammer, der er nævnt i aftalen. Undtaget herfra er korte uddrag til anmeldelse.
        </v-card-text>
      </v-card>
      
    </v-footer>
     
  </v-container>
  
</template>

<script>
export default {
  name: "Footer",

  data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>

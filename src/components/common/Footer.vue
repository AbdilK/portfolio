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

        <v-card-text class="amber--text pt-0">
          © 2021 Alle rettigheder forbeholdes ABDIL KOYCU
          <br>
          _________________________________________________________________________________________________________________________________________________________________
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Abdil Koycu's portfolio</strong>
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
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>

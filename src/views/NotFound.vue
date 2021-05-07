<template>
  <v-content>
    <v-container>
      <div class="section text-center notFound">
        <h2>Page not found</h2>
        <i class="fas fa-exclamation-triangle red--text"></i>
        <p>
          Beklager, men denne side findes ikke. Kontakt mig, også finder vi en
          løsning på dette..
        </p>
      </div>
    </v-container>
  </v-content>
</template>

<script>
export default {
  name: "NotFound",

  data() {
    return {
      items: [],
    };
  },
};
</script>
<template>
  <div class="section myStory">
    <v-container>
      <h2 class="text-center" amber accent-3>Mig og mit arbejde</h2>
      <h3 class="text-center">
        Jeg har de sidste par år hjulpet iværksættere og små virksomheder med
        grafisk design og hjemmesider – og jeg kan også hjælpe dig. Som grafisk
        designer og webdesigner har jeg hjulpet virksomheder i gang med deres
        forretning, branding og hjemmesider. Det har lært mig, at skal du skabe
        et perfekt fundament for din virksomhed. Der er 7 ingredienser, der skal
        til for at skabe et favoritbrand.
      </h3>
      <br />

      <h2 class="text-center" amber accent-3>
        Et æstetisk og strategisk favoritbrand er:
      </h2>
      <br />

      <p class="text-center">
        <strong>✔ SKARPT</strong>| Forstår de relevante personer klart, tydeligt
        og ikke mindste på et splitsekund, hvad du tilbyder? <br /><strong
          >✔ RELEVANT</strong
        >| Forstår og værdsætter de relevante personer, hvordan du kan hjælpe
        dem med det problem, de har? <br /><strong>✔ UNIKT</strong>| Genkender
        de relevante personer deres emotionelle udbytte, og ved de hvorfor du
        har den bedste løsning til netop dem? <br /><strong
          >✔ PASSIONERET </strong
        >| Ved de relevante personer, hvad du står for, og fornemmer de din
        passion? <br /><strong>✔ TROVÆRDIGHED </strong>| Tror de relevante
        personer på, at du kan levere det, du lover? <br /><strong
          >✔ UNIKT </strong
        >| Ved de relevante personer, at du eksisterer, og er du jævnligt synlig
        over for dem på relevante steder? <br /><strong>✔ KONSEKVENT</strong>|
        Er du så konsekvent og ensartet i din visuelle fremtoning, at de
        relevante personer genkender i et hvert touchpoint? <br /><br />
      </p>
      <h3 class="text-center">
        Hvis du har passionen, kan jeg hjælpe dig med resten.
      </h3>
      <br />
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
      ],
    };
  },
};
</script>
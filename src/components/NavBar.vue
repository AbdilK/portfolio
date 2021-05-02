<template >
  <v-container >
    <v-toolbar flat  >
      <v-toolbar-title >Portfolio</v-toolbar-title>

      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn text >
          HOME
        </v-btn>

        <v-btn text>
          ABOUT
        </v-btn>

        <v-btn text>
          CONTACT
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </v-container>
</template>

<script>
export default {
  name: "NavBar",

  data: () => ({}),
};
</script>

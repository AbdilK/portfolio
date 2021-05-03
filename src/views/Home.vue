<template>
  <v-content>
    <mySlide />
    <myPhotos />
    <myProjects />
  </v-content>
</template>

<script>
import mySlide from "../components/mySlide";
import myPhotos from "../components/myPhotos";
import myProjects from "../components/myProjects";

export default {
  name: "Home",

  components: {
    mySlide,
    myPhotos,
    myProjects
  }
};
</script>
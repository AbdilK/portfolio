<template>
  <v-content>

    <mySlide />
    <myStory />
    <myPhotos />
    <myProjects />
  </v-content>
</template>

<script>

import mySlide from "../components/mySlide";
import myStory from "../components/myStory";
import myPhotos from "../components/myPhotos";
import myProjects from "../components/myProjects";

export default {
  name: "Home",

  components: {
    mySlide,
    myStory,
    myPhotos,
    myProjects
  }
};
</script>
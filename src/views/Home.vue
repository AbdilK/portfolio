<template>
  <v-content>
    <mySlide />
    <myStory />
    <myProjects />
    <myPhotos />
  </v-content>
</template>

<script>
import mySlide from "../components/mySlide";
import myStory from "../components/myStory";
import myProjects from "../components/myProjects";
import myPhotos from "../components/myPhotos";

export default {
  name: "Home",

  components: {
    mySlide,
    myStory,
    myProjects,
    myPhotos,
  },
};
</script>
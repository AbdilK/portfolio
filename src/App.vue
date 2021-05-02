<template>
  <v-app>
    <v-app-bar 
      app
      flat
      
      
    >
    <NavBar/>
    </v-app-bar>

    <v-content>
      <imageSlide/>
      <imageGallery/>
      <imageProjects/>
    </v-content>

    <v-footer>
      <Footer/>
    </v-footer>
  </v-app>
</template>


<script>
import NavBar from './components/NavBar';
import imageSlide from './components/imageSlide';
import imageGallery from './components/imageGallery';
import imageProjects from './components/imageProjects';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    NavBar,
    imageSlide,
    imageGallery,
    imageProjects,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>

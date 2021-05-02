<template>
<div class="imageSlides">
  <v-carousel hide-delimiters cycle>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    >
    <v-row class="fill-height title" align="center" justify="center">
            <div>
              {{ item.title }}
            </div>
    </v-row>
  </v-carousel-item>
  </v-carousel>
  </div>
</template>

<script>
export default {
  name: "imageSlide",

  data () {
      return {
        items: [
          {
            src: require("../assets/images/test1.png"),
            title: ""
          },

          {
            src: require("../assets/images/img-carousel2.jpg"),
            title: "test2@@@@@@@@"
          },

          {
            src: require("../assets/images/img-carousel3.jpg"),
            title: "test3@@@@@@@@@"
          },
        ],
      }
    },
};
</script>

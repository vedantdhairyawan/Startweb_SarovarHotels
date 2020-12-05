<template>
  <v-carousel height="700px">
    <!-- carousel height -->
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
      eager
    ></v-carousel-item>
  </v-carousel>
  <!-- transition between carousel images fade while surfing back and forth-->
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'Taj Mahal.jpg',
          },
          {
            src: 'A.jpg',
          },
          {
            src: 'Agra Fort.jpg',
          },
          {
            src: 'Itimad-ud-Daulah.jpg',
          },
        ],
      }
    },
  }
</script>
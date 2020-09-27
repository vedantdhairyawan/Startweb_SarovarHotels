<template>
  <v-carousel class=" d-sm-none d-md-none d-lg-none">
  <!-- appears only on xs -->
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'Taj Mahal Dome - 1.jpg',
          },
          {
            src: 'Agra Fort.jpg',
          },
          {
            src: 'Taj Mahal Dome.jpg',
          },
          {
            src: 'A.jpg',
          },
        ],
      }
    },
  }
</script>
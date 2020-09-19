<template>
  <v-carousel>
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
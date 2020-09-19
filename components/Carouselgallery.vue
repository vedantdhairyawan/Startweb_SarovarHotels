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
            src: 'Dining area1.jpg',
          },
          {
            src: 'Pool2.jpg',
          },
          {
            src: 'Bedroom-3.jpg',
          },
          {
            src: 'Bedroom-4.jpg',
          },
        ],
      }
    },
  }
</script>
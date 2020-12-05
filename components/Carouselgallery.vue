<template>
  <v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
      eager
    >
    <!-- for loop for carousel images -->
    </v-carousel-item>
  </v-carousel>
</template>
<!-- v-model="valueDeterminate" -->
<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'Dining area1.jpg',
            // image-1 to be used in the carousel
          },
          {
            src: 'Pool2.jpg',
            // image-2 to be used in the carousel
          },
          {
            src: 'Bedroom-3.jpg',
            // image-3 to be used in the carousel
          },
          {
            src: 'Bedroom-4.jpg',
            // image-4 to be used in the carousel
          },
        ],
      }
    },
  }
</script>

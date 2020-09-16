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
            src: 'https://res.cloudinary.com/simplotel/image/upload/x_0,y_401,w_4368,h_2461,r_0,c_crop,q_80,fl_progressive/w_1500,c_fit,f_auto/nidhivan-sarovar-portico-vrindavan/Nidhivan_Back_Facade_wuqrys',
          },
          {
            src: 'https://cf.bstatic.com/images/hotel/max1280x900/148/148201887.jpg',
          },
          {
            src: 'https://i.ytimg.com/vi/vDhDhMtN92s/maxresdefault.jpg',
          },
          {
            src: 'https://www.crystalsarovaragra.com/images/skygrill.jpg',
          },
        ],
      }
    },
  }
</script>
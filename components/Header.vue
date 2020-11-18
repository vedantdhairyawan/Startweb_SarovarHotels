<template>
  <!-- <img
    class="Header"
    alt="Home"
    src="Header.png"
  > -->
</template>

<style>
/* .Header {
  height: 80px;
  width: 1000px;
    margin: 0 auto;
} */
</style>


<template>
  <v-footer
    dark
    padless
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="indigo">
         <img
            class="Header"
            alt="Home"
            src="sarovar1.png"
          >


        <v-spacer></v-spacer>

        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          dark
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-title>


    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-account',


      ],
    }),
  }
</script>

<style>
  .Header {
    height: 50px;
    width: 100px;
      margin: 0 auto;
  }
</style>


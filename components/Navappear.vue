<template>
  <v-bottom-navigation class="d-lg-none"
      fixed
      hide-on-scroll
      scroll-threshold="50"
      background-color="#0a4082"
      color="white"
    >
    <!-- d-lg-none, fixed-persistent, hide-on-scroll for hiding nav bar once a certain no of pixels are scrolled, sc
        scroll-threshold for mentioning no of pixels, bg color-nav bar color=brand color, on selection- color=white -->
    
      <v-btn href="holidays#ExploreAgra">
        <span>Explore Agra</span>
        <!-- text in button mentioned in span -->
        <!-- href for mentioning section that needs to be scrolled to -->
      </v-btn>

      <v-btn href="holidays#Location">
        <span>Location</span>
      </v-btn>

      <v-btn href="holidays#Dining">
        <span>Dining</span>
      </v-btn>

      <v-btn href="holidays#Gallery">
        <span>Gallery</span>
      </v-btn>
  </v-bottom-navigation>
</template>


<template>
  <v-row>
    <v-col cols="12" class="noscroll">
    <!-- applying class noscroll to make vertical scrollspy invisible in less than lg -->
      <div class="mx-10 my-2">
      <!-- defining margin in x axis and y axis respectively for horizontal and vertical spacing between buttons -->
        <v-btn class="text-center rounded-pill d-inline-flex"
          height="85"
          width="85"
          color="#0A4082"
          href="holidays#ExploreAgra">Explore <br> Agra
        </v-btn>
        <!-- rounded pill for circular button with equal height and width, href for linking to different sections of the page -->
      </div>
      
      <div class="mx-10 my-2">
        <v-btn class="text-center rounded-pill d-inline-flex"
          height="85"
          width="85"
          color="#0A4082"   href="holidays#Location">Location
        </v-btn>
      </div>
      
      <div class="mx-10 my-2">
        <v-btn class="text-center rounded-pill d-inline-flex"
          height="85"
          width="85"
          color="#0A4082"   
          href="holidays#Dining">Dining
        </v-btn>
      </div>
        
      <div class="mx-10 my-2">
        <v-btn class="text-center rounded-pill d-inline-flex"
          height="85"
          width="85"
          color="#0A4082"  href="holidays#Gallery" >Gallery</v-btn>
      </div>
      
    </v-col>
  </v-row>
</template>

<style>
@media (max-width: 1160px) {
.noscroll {
display: none
}}
/* after screen size max width is less than 1160px, vertical scrollspy will vanish */
</style>
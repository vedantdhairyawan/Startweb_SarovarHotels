<template>
  <html class="noscrollbar">
    <head>
      <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
      <!-- linking to materialize library of icons -->
    </head>
      
      <v-tabs
      light
      color="#0a4082"
      left
      >
      <!-- light theme -->
      <!-- color for icon color -->
      <!-- left aligning tab icons -->

        <v-tab> <i class="material-icons">photo_size_select_actual</i></v-tab>
        <v-tab> <i class="material-icons">location_on</i></v-tab>
        <v-tab><i class="material-icons">satellite</i></v-tab>
        <!-- icons for tabs -->

        <v-tab-item>
          <Growshrink/>
          <!-- Gallery for first tab -->
          <Carousellocationxs/>
          <!-- for inserting location related images on xs -->
        </v-tab-item>


        <v-tab-item>
          <v-img
          src="Maplocation.jpg" >
          </v-img>
          <!-- map image for second tab -->
        </v-tab-item>

        <v-tab-item>
          <v-img
          src="Satellite.jpg" >
          </v-img>
          <!-- satellite image for third tab -->
        </v-tab-item>
      </v-tabs>
  
  </html>
</template>

<style>
.noscrollbar{
overflow-y: hidden;}
/* hiding vertical scrollbar */
</style>


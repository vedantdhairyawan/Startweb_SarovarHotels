<template>
  <html class="noscrollbar">
    <head>
      <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
      <!-- linking to materialize library of icons -->
    </head>
    <v-card>
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


        <v-tab-item eager height="550px">
          <v-img
          src="Maplocation.jpg" 
          lazy-src="Maplocation.jpg"
          aspect-ratio="2.6"
          height="400px" >

          <template v-slot:placeholder>
          <v-row
            class="fill-height ma-0"
            align="center"
            justify="center"
          >
            <v-progress-circular
              indeterminate
              color="grey lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
          </v-img>
          <!-- map image for second tab -->
        </v-tab-item>

        <v-tab-item eager height="550px">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d109586.5980917848!2d77.90997246073701!3d27.176309822555126!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39740d857c2f41d9%3A0x784aef38a9523b42!2sAgra%2C%20Uttar%20Pradesh!5e1!3m2!1sen!2sin!4v1608456887439!5m2!1sen!2sin" width="1200" height="550" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>          <!-- satellite image for third tab -->
        </v-tab-item>
      </v-tabs>
    </v-card>
  
  </html>
</template>

<style>
.noscrollbar{
overflow-y: hidden;}
/* hiding vertical scrollbar */

</style>


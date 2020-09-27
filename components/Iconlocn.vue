<template>
  <html class="noscrollbar">
    <head>
      <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
      <!-- linking to materialize library of icons -->
    </head>
    
      <v-tabs
        v-model="tab"
        background-color="white"
        color="#0a4082"
        left
        light
        >
      <!-- bg color of button=white, icon-color=brand color,  left aligned buttons, light theme, -->
      
      <v-tabs-slider></v-tabs-slider>
        
          <v-tab href="#tab-1">
            <i class="material-icons">photo_size_select_actual</i>
            <!-- icon-gallery -->
          </v-tab>

          <v-tab href="#tab-2">
            <i class="material-icons">location_on</i>
            <!-- icon-location -->
          </v-tab>

          <v-tab href="#tab-3">
            <i class="material-icons">satellite</i>
            <!-- icon-satellite -->
          </v-tab>
      
      </v-tabs>
 </html>
</template>

<style>
.noscrollbar{
overflow-y: hidden;}
/* hiding vertical scrollbar */
</style>
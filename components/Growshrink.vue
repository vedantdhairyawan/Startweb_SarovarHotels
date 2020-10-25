<template>
  <v-container class="background">
    <div>
      <v-row class="d-none d-sm-flex d-md-flex d-lg-flex">
      <!-- disappears on xs  -->
        <v-col cols="8" sm="9" md="9">
          <v-img
          height="550px" 
          src="Taj Mahal Dome - 1.jpg" >
          </v-img>
        </v-col>
          <!-- image height of Taj Mahal to be 3x height of the adjacent images -->
      
      <v-col cols="4" sm="3" md="3" offset-md="0.1">
        <!-- offset for horizontal spacing  -->
        <v-row 
        :align="align"
        no-gutters
        style="height: 185px;">
        <!-- vertical spacing -->
          <v-img 
            height="180px"
            src="Agra Fort.jpg"
          > </v-img>
        </v-row>
            
        <v-row 
          :align="align"
          no-gutters
          style="height: 185px;">
          <v-img
            height="180px"
            src="Taj Mahal Dome.jpg"
          > </v-img>
        </v-row>

          <v-img
            height="180px"
            src="A.jpg"
          > </v-img>
          <!-- v-img to insert images -->
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<style>
  .background{background-color: white;}
</style>

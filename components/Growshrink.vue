<template>
  <v-container>
    <v-row class="mb-6">
      <v-col cols="12" md=9>
        <v-img
        height="550px" 
        src="Taj Mahal Dome - 1.jpg" >
        </v-img>
      </v-col>
        
        <!-- image height of Taj Mahal to be 3x height of the adjacent images + -->
        <v-col cols="12" md="3" offset-md="0.1">
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
          
        
        </v-col>
    </v-row>
  </v-container>
</template>

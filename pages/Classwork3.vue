<template>
  <v-container>
   <v-row
      no-gutters
      >
      <v-col
      v-for="j in 3"
      :key= j
      cols="12"
      md="4"
      >


      <v-card
        class="pa-2 md-1"
        color="black"
        >
        <v-card-text class="yellow--text">
          Adjust screen size to see spacing changes
        </v-card-text>
      </v-card>


      </v-col>
    </v-row>


  </v-container>
</template>

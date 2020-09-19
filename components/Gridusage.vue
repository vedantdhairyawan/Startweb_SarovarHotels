<template>
  <v-container class="grey lighten-5">
    <v-row no-gutters>
      <!-- no gutters removes spacing between elements -->
      <v-col
        v-for="n in 6"
        :key="n"
        cols="12"
        sm="4"
        md="4"
      >
        <v-card
          class="pa-7"
          outlined
          tile
        >
        <!-- pa for padding -->
          One of three columns
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
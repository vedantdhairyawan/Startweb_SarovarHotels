<template>
  <v-container class="grey lighten-5">
    <v-row
      class="mb-6"
      no-gutters
    >
      <v-col
        v-for="n in 3"
        :key="n"
        :cols="n === 2 ? 6 : undefined"
      >
      <!-- === is a tertiary operator that verifies value and type of value -->
        <v-card
          class="pa-2"
          outlined
          tile
        >
          {{ n }} of 3 {{ n === 2 ? '(wider)' : '' }}
        </v-card>
      </v-col>
    </v-row>
    <v-row no-gutters>
      <v-col
        v-for="n in 3"
        :key="n"
        :cols="n === 2 ? 5 : undefined"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          {{ n }} of 3 {{ n === 2 ? '(wider)' : '' }}
        </v-card>
      </v-col>
    </v-row>

    <v-row no-gutters>
      <v-col
        v-for="n in 7"
        :key="n"
        :cols="n === 1 ? 12 : undefined"
      >
      <!-- n===2 is which part and 5 is how wide -->
      <!-- ? is if then -->
        <v-card
          class="pa-2"
          outlined
          tile
        >
          {{ n }} of 3 {{ n === 2 ? '(wider)' : '' }}
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<template>
  <v-container class="grey lighten-5">
    <v-row
      v-for="n in 7"
      :key="n"
      :class="n === 1 ? 'mb-6' : ''"
      no-gutters
    >
    <!-- mb is for bottom margin when n i.e row is the first one -->
      <v-col
        v-for="k in n + 1"
        :key="k"
        >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          {{ k }} of {{ n + 1 }}
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
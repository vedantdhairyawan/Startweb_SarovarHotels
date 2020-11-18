<template>
  <v-container class="white ma-1 pa-lg-2 pa-md-4 pa-sm-2"
  max-height="220px"
  lg="10"
  md="8"
  sm="4"
  xs="2"


  >
   <v-row justify="center"
      no-gutters
      >
      <!-- Birthdays radio button -->
      <v-col
      cols="12"
      md="3"
      sm="2"
      xs="1"
      class="ma-1 pa-lg-2 pa-md-4 pa-sm-2"
      >

        <v-card
          class="grey"
          max-width="200px"
        >

          <v-radio-group>
            <v-radio label="Birthdays" value="radio-1" ></v-radio>

          </v-radio-group>


        </v-card>

      </v-col>

      <!-- Workshops radio button -->
      <v-col
      cols="12"
      md="3"
      sm="2"
      xs="1"
      class="ma-1 pa-lg-2 pa-md-4 pa-sm-2"
      >

        <v-card
          class="grey"
          max-width="200px"
        >

          <v-radio-group>
            <v-radio label="Workshops" value="radio-2" ></v-radio>

          </v-radio-group>


        </v-card>

      </v-col>

      <!-- Parties radio button -->
      <v-col
      cols="12"
      md="3"
      sm="2"
      xs="1"
      class="ma-1 pa-lg-2 pa-md-4 pa-sm-2"
      >

        <v-card
          class="grey"
          max-width="200px"
        >

          <v-radio-group>
            <v-radio label="Parties" value="radio-3" ></v-radio>

          </v-radio-group>


        </v-card>

      </v-col>
    </v-row>

    <v-row justify="center"
      no-gutters
      >
      <!-- weddings radio button -->
      <v-col
      cols="12"
      md="3"
      sm="2"
      xs="1"
      class="ma-1 pa-lg-2 pa-md-4 pa-sm-2"
      >

        <v-card
          class="grey"
          max-width="200px"
        >

          <v-radio-group>
            <v-radio label="Weddings" value="radio-4" ></v-radio>

          </v-radio-group>


        </v-card>

      </v-col>

      <!-- launch events radio button -->
      <v-col
      cols="12"
      md="3"
      sm="2"
      xs="1"
      class="ma-1 pa-lg-2 pa-md-4 pa-sm-2"
      >

        <v-card
          class="grey"
          max-width="200px"
        >

          <v-radio-group>
            <v-radio label="Launch Events" value="radio-5" ></v-radio>

          </v-radio-group>


        </v-card>

      </v-col>

      <!-- ceremonies radio button -->
      <v-col
      cols="12"
      md="3"
      sm="2"
      xs="1"
      class="ma-1 pa-lg-2 pa-md-4 pa-sm-2"
      >

        <v-card
          class="grey"
          max-width="200px"
        >

          <v-radio-group>
            <v-radio label="Ceremonies" value="radio-6" ></v-radio>

          </v-radio-group>


        </v-card>

      </v-col>
    </v-row>


  </v-container>
</template>

<script>
  export default {
    data () {
      return {
        column: true,
        row: false,
      }
    },
  }
</script>

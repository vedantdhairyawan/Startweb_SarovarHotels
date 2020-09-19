<template>
  <v-container fluid>
    <!-- responsive container -->
    <v-row>
      <v-col cols="12">
        <!-- changing columns will restrict the movement of alignment and justification to that number of columns -->
        <v-row
          :align="alignment"
          :justify="justify"
          class="grey lighten-5"
          style="height: 300px;"
        >
        <!-- align vertical, justify horizontal -->
        <!-- specifying align as alignment and justify as justify calls the buttons assigned 
             the respective properties to act on the rows alignment -->
          <v-card
            v-for="n in 3"
            :key="n"
            class="ma-3 pa-6"
            outlined
            tile
          >
            Column
          </v-card>
        </v-row>
      </v-col>
      <v-col cols="12">
        <v-row justify="center">
          <v-col
            cols="6"
            md="2"
          >
            <v-select
              v-model="alignment"
              :items="alignmentsAvailable"
              label="Align"
              background-color="black"
            ></v-select>
            <!-- v select for selecting alignment options -->
          </v-col>

          <v-col
            cols="6"
            md="2"
          >
            <v-select
              v-model="justify"
              :items="justifyAvailable"
              label="Justify"
            ></v-select>
            <!-- v-select enables selecting of justify options  -->
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    data () {
      return {
        alignmentsAvailable: [
          'start',
          'center',
          'end',
          'baseline',
          'stretch',
        ],
        alignment: 'center',
        dense: false,
        justifyAvailable: [
          'start',
          'center',
          'end',
          'space-around',
          'space-between',
        ],
        justify: 'center',
      }
    },
  }
</script>

<template>
  <v-row justify="center">
    <v-dialog v-model="dialog" persistent max-width="290">
      <!-- persistent for making the box stay even after clicking outside -->
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Open Dialog
        </v-btn>
      </template>
      <v-card>
        <v-card-title class="headline">Use Google's location service?</v-card-title>
        <!-- card header -->
        <v-card-text>Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <!-- to leave vertical spacing between elements -->
          <v-btn color="green darken-1" text @click="dialog = false">Disagree</v-btn>
          <v-btn color="green darken-1" text @click="dialog = false">Agree</v-btn>
          <!-- on clicking the options, the boolean operation makes the box disappear -->
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
  export default {
    data () {
      return {
        dialog: false,
        // box does not activate at initialization
      }
    },
  }
</script>
<template>
  <div class="text-center">
    <v-dialog
      v-model="dialog"
      width="500"
    >
    <!-- v-model for binding a form input element and making it change its property when it is selected -->
    <!-- dimensions and text alignment -->
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="red lighten-2"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Click Me
        </v-btn>
      </template>
      <!-- v-on for events to be activated -->

      <v-card>
        <v-card-title class="headline grey lighten-2">
          Privacy Policy
        </v-card-title>
        <!-- card header -->

        <v-card-text>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </v-card-text>
        <!-- card paragraph -->

        <v-divider></v-divider>
        <!-- dividers -->

        <v-card-actions>
          <v-spacer></v-spacer>
          <!-- vertical spacing -->
          <v-btn
            color="primary"
            text
            @click="dialog = false"
          >
          <!-- clicking makes it disappear -->
            I accept
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        dialog: false,
        // disabled at webpage initialiation 
      }
    },
  }
</script>
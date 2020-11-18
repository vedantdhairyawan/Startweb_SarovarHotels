<template>
    <v-container id="dropdown-example">
      <v-row>


        <v-col cols="12" sm="4">

        <!-- dropdowns for catering -->
        <!-- font color tag has been used to change the color of text -->

          <font color="#BDBDBD">
            <h2>1. Catering</h2>
          </font>
          <v-overflow-btn
            class="my-2 blue"
            :items="dropdown_edit"
            label="Options"
            item-value="text"
          ></v-overflow-btn>
        </v-col>
      </v-row>

      <!-- dropdowns for stewards -->

      <v-row>
        <v-col cols="12" sm="4">

          <font color="#BDBDBD">
            <h2>2. Stewards</h2>
          </font>

          <v-overflow-btn
            class="my-2 blue"
            :items="steward_number"
            label="Options"
            item-value="text"
          ></v-overflow-btn>
        </v-col>
      </v-row>

      <!-- dropdowns for sound equipment -->

      <v-row>
        <v-col cols="12" sm="4">

          <font color="#BDBDBD">
            <h2>3. Sound Equipment</h2>
          </font>

          <v-overflow-btn
            class="my-2 blue"
            multiple
            :items="sound"
            label="Options"
            item-value="text"
          ></v-overflow-btn>
        </v-col>
      </v-row>

    </v-container>
</template>

<script>

  // To call data you need to put everything between these brackets []

  export default {
    data: () => ({

      dropdown_edit: [
        { text: 'Vegetarian' },
        { text: 'Non-Vegetarian' },
      ],
      steward_number: [
        { text: '5' },
        { text: '10' },
        { text: '15' },
      ],
      sound: [
        { text: 'Speakers' },
        { text: 'Microphones' },
      ],
    }),
  }


</script>

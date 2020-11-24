<template>
    <v-container class="white" id="dropdown-example">
      <v-row>


        <v-col cols="12" sm="4">

        <!-- dropdowns for catering -->

          <v-checkbox color="white"
            <font color="#BDBDBD">
              <h3>Number of Tables</h3>
            </font>
          <v-overflow-btn
            light
            background-color="#E3F2FD"
            color="#0a4082"
            outlined
            class="my-2"
            editable
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
              <h3>Number of Chairs</h3>
            </font>

          <v-overflow-btn
            class="my-2"
            light
            background-color="#E3F2FD"
            outlined
            color="#0a4082"
            editable
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
              <h3>Number of Screens</h3>
            </font>

          <v-overflow-btn
            class="my-2"
            light
            color="#0a4082"
            background-color="#E3F2FD"
            outlined
            editable
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
        { text: '20-30' },
        { text: '30-40' },
        { text: '40-50' },
      ],
      steward_number: [
        { text: '20-30' },
        { text: '30-40' },
        { text: '40-50' },
      ],
      sound: [
        { text: '2' },
        { text: '4' },
        { text: '8' },
      ],
    }),
  }


</script>


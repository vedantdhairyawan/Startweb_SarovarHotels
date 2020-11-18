<template>
  <v-container class="white" id="dropdown-example">

    <v-row>
        <v-col cols="12" sm="4">
          <font color="#BDBDBD">
            <h2>Estimated Number of People</h2>
          </font>

        <v-overflow-btn
          class="my-2 blue"
          :items="dropdown_edit"
          label="Choose"
          editable
          outlined
          item-value="text"
        ></v-overflow-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      dropdown_edit: [
        { text: '20-30' },
        { text: '30-40' },
        { text: '40-50' },

      ],
    }),
  }
</script>

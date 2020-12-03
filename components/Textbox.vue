<template>
  <v-form>
    <v-container>
      <v-row>

        <!-- This component is the "Queries Section"
        it has header text in blue an grey color
        those headers have editable text boxes, that work under them -->


        <v-col
          cols="12"
          sm="6"
        >
        <!-- Bold Heads -->
          <font color="#BDBDBD">
            <h2>Queries? Contact Us...</h2>
          </font>

          <!-- Normal sized heads -->
          <font color="#1565C0">
            <h4>E-mail / Phone Number</h4>
          </font>

          <v-text-field light
            background-color="#E3F2FD"
            color="#0a4082"
            label="example@gmail.com / 98xxxxxxxx"
            single-line
            outlined

          ></v-text-field>
        </v-col>

      </v-row>

      <v-row>

        <v-col
          cols="12"
          sm="6"
        >
          <font color="#1565C0">
            <h4>Queries</h4>
          </font>
          <v-text-field light
            background-color="#E3F2FD"
            color="#0a4082"
            label="Type Here..."
            single-line
            outlined
          ></v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>

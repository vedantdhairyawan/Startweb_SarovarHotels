<template>
<!-- stepper form was used to make my web-page as it was the perfect component to use for my idea -->
  <v-container class="white" md="12" sm="8" xs="12">

    <font color="#0a4082">
      <h1>Hall Booking</h1>
    </font>

    <v-col cols="12">

      <v-stepper class="white" v-model="e6" vertical>
        <v-stepper-step :complete="e6 > 1" step="1">
          <font color="#0a4082">
            <h2>Type of Event</h2>
          </font>
          <small></small>
        </v-stepper-step>

        <v-stepper-content step="1">
          <v-card color="white" class="mb-12" flat>

            <!-- Contents of "Types of Event"  -->

            <Radiobuttons/>

          </v-card>
          <v-btn color="#0a4082" @click="e6 = 2">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <!-- this section adds elements below v-card -->

        <v-stepper-step :complete="e6 > 2" step="2">
          <font color="#0a4082">
            <h2>Specifications</h2>
          </font>
          </v-stepper-step>

        <v-stepper-content step="2">
          <v-card outlined class="mb-12">

            <!-- Contents of "Specifications"  -->

            <Dropdowns/>
            <Checkboxe1/>

          </v-card>
          <v-btn color="#0a4082" @click="e6 = 3">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <v-stepper-step :complete="e6 > 3" step="3">
          <font color="#0a4082">
            <h2>Hall Suggestions</h2>
          </font>
          </v-stepper-step>

          <!-- the feature "outlined" worked for step 4 of the stepper form -->

        <v-stepper-content step="3">
          <v-card outlined class="mb-12" light>

            <!-- Contents of "Hall Suggestions"  -->

            <!-- <HorizontalCard/> -->

            <!-- add margin spacing -->

            <HorizontalCard/>
            <HorizontalCard/>


          </v-card>
          <v-btn color="#0a4082" @click="e6 = 4">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <v-stepper-step step="4">
          <font color="#0a4082">
            <h2>Optional Extras</h2>
          </font>
          </v-stepper-step>
          <!-- In the same manner "Outlined" was used again in exactly the same way, but it did not work -->
        <v-stepper-content step="4">
          <v-card  light class="mb-12" height="750px">

              <Dropdowns2/>
              <Textbox/>

          </v-card>
          <v-btn color="#0a4082" @click="e6 = 5">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <v-stepper-step step="5">
          <font color="#0a4082">
            <h2>Confirmation</h2>
          </font>
          </v-stepper-step>
        <v-stepper-content step="5">
          <!-- again "outlined" did not work here -->
          <v-card  light class="mb-12" flat>

            <!-- Contents of "Confirmation"  -->

            <ConfirmForm/>


          </v-card>
          <v-btn color="#0a4082" @click="e6 = 1">Confirm</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

      </v-stepper>
    </v-col>
  </v-container>
</template>

// add scripts in sequence

<script>
    // script for stepper form
  export default {
    data () {
      return {
        e6: 1,
      }
    },
  }
</script>




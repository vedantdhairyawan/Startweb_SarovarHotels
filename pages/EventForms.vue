<template>
<!-- stepper form was used to make my web-page as it was the perfect component to use for my idea -->
  <v-container class="white" md="12" sm="8" xs="12">

    <h1>Hall Booking</h1>

    <v-col cols="12">

      <v-stepper class="white" v-model="e6" vertical>
        <v-stepper-step :complete="e6 > 1" step="1">
          <h2 class="blue--text">Type of Event</h2>
          <small></small>
        </v-stepper-step>

        <v-stepper-content step="1">
          <v-card color="white" class="mb-12" height="450px">

            <!-- Contents of "Types of Event"  -->

            <Radiobuttons/>

          </v-card>
          <v-btn color="primary" @click="e6 = 2">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <!-- this section adds elements below v-card -->

        <v-stepper-step :complete="e6 > 2" step="2">
          <h2 class="blue--text">Specifications</h2>
          </v-stepper-step>

        <v-stepper-content step="2">
          <v-card outlined class="mb-12" height="675px">

            <!-- Contents of "Specifications"  -->

            <Dropdowns/>
            <Checkboxe1/>

          </v-card>
          <v-btn color="primary" @click="e6 = 3">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <v-stepper-step :complete="e6 > 3" step="3">
          <h2 class="blue--text">Hall Suggestions</h2>
          </v-stepper-step>

          <!-- the feature "outlined" worked for step 4 of the stepper form -->

        <v-stepper-content step="3">
          <v-card outlined class="mb-12" height="630px">

            <!-- Contents of "Hall Suggestions"  -->

            <!-- <HorizontalCard/> -->

            <!-- add margin spacing -->

            <HorizontalCard/>
            </br>
            <HorizontalCard/>


          </v-card>
          <v-btn color="primary" @click="e6 = 4">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <v-stepper-step step="4">
           <h2 class="blue--text">Optional Extras</h2>
          </v-stepper-step>
          <!-- In the same manner "Outlined" was used again in exactly the same way, but it did not work -->
        <v-stepper-content step="4">
          <v-card outlined color="#F5F5F5" class="mb-12" height="750px">

              <Dropdowns2/>
              <Textbox/>

          </v-card>
          <v-btn color="primary" @click="e6 = 5">Confirm & Continue</v-btn>
          <!-- <v-btn text>Cancel</v-btn> -->
        </v-stepper-content>

        <v-stepper-step step="5">
          <h2 class="blue--text">Confirmation</h2>
          </v-stepper-step>
        <v-stepper-content step="5">
          <!-- again "outlined" did not work here -->
          <v-card outlined color="#F5F5F5" class="mb-12" height="550px">

            <!-- Contents of "Confirmation"  -->

            <ConfirmForm/>


          </v-card>
          <v-btn color="primary" @click="e6 = 1">Confirm</v-btn>
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




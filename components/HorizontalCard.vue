<template>
<!-- cards work very well in "lg" view but even after a lot of tries, was not able to make them responsive for mobile -->
  <v-card class="col-12 ml-0" sm="3" color="#E3F2FD" background-color="#E3F2FD" outlined max-height="300px" md="4">
    <v-container fluid class="ml-2">
      <v-row justify="space-between">
        <v-col cols="12"
          md="5"
        >
            <v-carousel height="200">
              <v-carousel-item
                v-for="(item,i) in items"
                :key="i"
                :src="item.src"
                reverse-transition="fade-transition"
                transition="fade-transition"
              ></v-carousel-item>
            </v-carousel>
        </v-col>

        <!-- card for name and address text -->
        <!-- remove elevation -->
       <v-col>
          <v-card
            color="#E3F2FD"
            background-color="#E3F2FD"
            max-width="190px"
            max-height="300"
            elevation="1"
            md="4"
            cols="12"
          >
            <v-container>
              <font color="#0a4082">
                <h3>Sarovar Portico</h3><br/>
                <h4 class="black--text">Carol Bagh, New Delhi</h4>
              </font>
            </v-container>
          </v-card>
       </v-col>

        <!-- card for availability text -->

       <v-col>
          <v-card
            color="#E3F2FD"
            max-width="190px"
            max-height="300"
            elevation="1"
            ml="10"
          >
            <v-container>
              <font color="#0a4082">
                <h3>Availability</h3><br/>
              </font>
              <v-card light outlined>
                <v-card-text>Available for 5 hours</v-card-text>

              </v-card>
            </v-container>
          </v-card>
       </v-col>

       <!-- card for specification text -->

       <v-col>
          <v-card
            color="#E3F2FD"
            max-width="190px"
            max-height="300"
            elevation="1"
            ml="10"
          >
            <v-container>

            <font color="#0a4082">
              <h3>Specifications</h3><br/>
            </font>
              <v-card light outlined>
                <v-icon class="mx-2">mdi-account</v-icon>
                <v-card-text>40-50</v-card-text>
                <v-card-text>Air Conditioning available</v-card-text>

              </v-card>

            </v-container>
          </v-card>
       </v-col>


        <!-- card for icons text -->
        <v-col
          cols="auto"
          class="text-center pl-0">
          <v-row
            class="flex-column ma-0 fill-height"
            justify="center"
          >
            <v-col class="px-0">

                <v-icon></v-icon>

            </v-col>

            <v-col class="px-0">

                <v-icon></v-icon>

            </v-col>

            <v-col class="px-0">
              <div class="my-2">
                <v-btn elevated small color="indigo">Choose</v-btn>
              </div>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://5.imimg.com/data5/SV/DX/GLADMIN-33559172/conference-hall-500x500.jpg',
          },
          {
            src: 'https://www.sinclairshotels.com/assets/images/burdwan/Regal-Room-l-and-ll.jpg',
          },
          {
            src: 'https://media-cdn.tripadvisor.com/media/photo-s/0b/51/39/62/conference-hall.jpg',
          },
          {
            src: 'https://www.thelalit.com/wp-content/uploads/2017/02/glance-kolkata3-760-320.jpeg',
          },
        ],
      }
    },
  }
</script>

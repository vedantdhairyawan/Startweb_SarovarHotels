<template>
  <div>
  
  <v-content>
    <carousel/>
    <!--Adds carousal images-->
   
  <v-container>
      <v-col cols="12" md="12"
      >
       
      <v-card
      class=" blue darken-4 mb-12 mt-6 pa-md-2 pa-sm-2 py-16 rounded-pill"
      outlined
      tiled
      
      >
      
        <v-card-title>
          <span class="headline"></span>
          <!--adds header/title to the card-->
        </v-card-title>
        <v-card-text>
          
            <v-row >  
            <!--Autocomplete and dropdown for searching location-->
              <v-col cols="10" md="3" sm="4"
              class="ml-md-16 ml-sm-16 ml-6
                     mt-md-n6 mt-sm-n6 mt-n8"
                     >
              <!--v-icon large color="white">mdi-city</v-icon-->
                <v-autocomplete
                
                  :items="['Agra', 'Delhi', 'Mumbai', 'Tirupati', 'Jalgaon', 'Tiruvantampuram', 'Ratnagiri', 'Thane', 'Banglore']"
                  label="Destinations"
                  prepend-icon="mdi-city"
                  colour="blue"
                  menu-props="light"
                  

                ></v-autocomplete>
              </v-col>
              <!--datepicker-->
              <v-col cols="10" md="2" sm="4"
              class="ml-md-2 ml-sm-2 ml-6
                     mt-md-n6 mt-sm-n6 mt-n6"
                     
             >
            

                <v-menu
        v-model="menu2"
        :close-on-content-click="true"
        :nudge-right="40"
        transition="scale-transition"
        offset-y
        min-width="290px"
      >
        <template v-slot:activator="{ on, attrs }">
          <v-text-field
            v-model="date"
            label="Date"
            prepend-icon="mdi-calendar"
            readonly
            v-bind="attrs"
            v-on="on"
            
          ></v-text-field>
        </template>
        <v-date-picker
          v-model="date"
          @input="menu2 = true"
          header-color="white"
          light
          
        ></v-date-picker>
      </v-menu>
                
              </v-col>
              <!--dropdown for services-->
              <v-col cols="10" md="2" sm="4"
              class="ml-md-2  ml-sm-16 ml-6
                     mt-md-n6 mt-sm-n6 mt-n6">
              <!--defines columns used and their position-->
                <v-autocomplete
                  :items="services"
                  label="Services"
                  item-text="name"
                  item-value="id"
                  return-object
                  v-model="selectedService"
                  
                  prepend-icon="mdi-call-split"
                  menu-props="light"
                  
                ></v-autocomplete>
              </v-col>
              <!--Autocomplete and dropdown for searching location-->
              
              <v-col cols="7" md="2" sm="4"
              class="ml-md-3 ml-sm-2 ml-6
                     mt-md-n6 mt-sm-n6 mt-n6">
                <v-autocomplete
                  :items="['1', '2', '3', '4', '5']"
                  
                  label="Occupancy"
                  prepend-icon="mdi-account"
                  menu-props="light"
                  
                  
                ></v-autocomplete>
              </v-col>
              <v-col cols="3" md="2" sm="2" >
              <div class="ml-md-4 ml-sm-4 
                          mt-md-n6 mt-sm-n14 mt-n6" >
            
            <template>
              <v-btn
                color="blue darken-4"
                fab
                large
                dark
                menu-props="light"
                :href="`${selectedService.link}`"
              >
                <v-icon>mdi-magnify</v-icon>
              </v-btn>
            </template>
          </div>
              <!--v-btn icon>
        <v-icon large color="white">mdi-action-search</v-icon>
      </v-btn-->
          </v-col>
            </v-row>
          
          
        </v-card-text>
      </v-card>
      </v-col>
      </v-container>
  <offer/>
  <!--images-->
  <low/>
  </v-content>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        date: new Date().toISOString().substr(0, 10),
        menu: false,
        modal: false,
        menu2: false,
        services: [{id: 1, name: "Events", link:"EventForms"}, {id: 2, name: "Holidays", link:"holidays"}
          ],
        selectedService: {id: null, name: null, link: ""}
      }
    },
    mounted() {
      this.selectedService = {id: null, name: null, link: ""}
    },
    methods: { 
      isEvents() {
        console.log("retu", this.selectedService.id == 1)
        return this.selectedService.id == 1
      }
    },
  }
</script>



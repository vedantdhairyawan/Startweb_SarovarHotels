<template>
  <div>
    <v-col cols="12">
      <v-sheet
          elevation="6"
          class="navbar"
          color="white"
        >
        <!-- To add a sheet with a dropshadow that is controlled by the elevation behind the scrollspy -->
        <!-- class="navbar" binds the scrollspy to the sheet-->
    <Scrollspyfunction/>
    </v-sheet>
    </v-col>      

      <v-col cols="12" sm="6" md="12">
        <Breadcrumb/>
        <!-- Breadcrumb component -->
          <section id="ExploreAgra" >
          <!-- section id ExploreAgra binds the section of the page to the Explore Agra link in the scrollspy--> 
            <Carouselmonuments/>
            <!-- Carousel component - monument pictures -->
            <!-- v-col defines number of columns, md defines size on medium screens -->
          </section>
      </v-col>
        
    
    <v-container>
      <!-- container enables centering the site's componenents in a grid -->
        <v-content>
         
          <v-col cols="12" sm="6" md="12">
            <v-row justify="center">
              <h1> Explore Agra </h1>
            </v-row>  
            <!-- Explore Agra justified in the center, h1 for larger size of heading -->
                <h2>The Magnificent Taj Mahal</h2>   
                    <!-- h2 for a smaller size of heading in comparison with h1  -->
                  <p> 
                    As part of India's golden triangle, the city of Agra is one of the travel hotspots of the world. 
                    Agra, home to the Taj Mahal, one of the seven wonders of the world, is rich in its history and architecture. 
                    Taj Mahal, an epitome of love, is regarded as an astounding architectural beauty and has continuously 
                    been on the 'Seven Wonders of the World' list. Taj Mahal was constructed for a period of 22 years, and 
                    a total of about twenty thousand workers were employed to build it. This architectural marvel is built entirely of 
                    white marble and it glows in the moonlight. Shah Jahan built this monument in the memory of his wife Mumtaz, 
                    whose grave is housed within the premises of the Taj Mahal. There are several other aspects that create the 
                    spectacle that the Taj Mahal is — beautiful Charbaghs(Taj Garden), the magnificent Darwaza,the symmetrical 
                    sandstone structures surrounding the Taj, and the placid Yamuna river that flows behind it.
                  </p>
                  <!-- paragraph tag -->
          </v-col>
        

          <section id="Location">
              <!-- section id Location binds the section of the page to the Location link in the scrollspy-->
            <v-col cols="12" sm="6" md="12">
              <v-row justify="center">
                  <h1>Location</h1>
              </v-row>
            </v-col>
              <Growshrink/>
          </section>

          <section id="Dining">
              <!-- section id Dining binds the section of the page to the Dining link in the scrollspy-->
            <v-col cols="12" sm="6" md="12">
              <v-row justify="center">
                <h1> Dining </h1>
                  <p align="center"> 
                    We love to eat, to take our time and enjoy the flavours in a series of small dishes. Our degustation gives you the chance to do exactly that. 
                    More than a succession of plates, we offer you an experience, a connection between each dish, pulling from a wide range of authenticities.
                  </p>
                  <!-- aligning paragraph to the center -->
              </v-row>
            </v-col>
    

              <v-row justify="left">
                <v-col cols="12" sm="6" md="5">
                  <v-img src="Cuisine meat 2.jpg" ></v-img>
                </v-col>
                <!-- v-img to insert images sourced from static folder -->
                <!-- justify left for images -->

                  <v-col cols="12" sm="6" md="7">
                    <h3>Assorted Barbecue Cuisine</h3>
                    <!-- h3 header size lower than h2 and h1 -->
                      <p> Passion is the most important ingredient, and we bring you the 
                          beauty of barbecue flavours in every bite. Owing to our expert chefs, 
                          a nightly-changing tasting menu is sure to take your taste-buds on an 
                          adventurous ride into the beauty of the charcoal taste of barbecue food. 
                      </p>
                  </v-col>
              </v-row>

              <v-row justify="left">
                <v-col cols="12" sm="6" md="5">
                  <v-img src="Cuisine French.jpg" ></v-img>
                </v-col>

                <v-col cols="12" sm="6" md="7">
                <h3>French Cuisine</h3>
                  <p> Passion is the most important ingredient, and we bring you 
                      the beauty of Italian flavours in every bite. Owing to our expert chefs, 
                      a nightly-changing tasting menu is sure to take your taste-buds on an 
                      adventurous ride into the beauty of Italian food. 
                  </p>
                </v-col>
              </v-row>

              <v-row justify="left">
                <v-col cols="12" sm="6" md="5">
                  <v-img src="Cuisine Italian.jpg" ></v-img>
                </v-col>

                <v-col cols="12" sm="6" md="7">
                  <h3>Italian Cuisine</h3>
                  <p>Passion is the most important ingredient, and we bring you 
                    the beauty of Mexican flavours in every bite. Owing to our expert chefs, 
                    a nightly-changing tasting menu is sure to take your taste-buds on an 
                    adventurous ride into the beauty of Mexican food.</p>
                </v-col>
              </v-row>
          </section>   
              
          <section id="Gallery">
              <!-- section id Gallery binds the section of the page to the Gallery link in the scrollspy-->
            <v-row justify="center">
              <h2>Gallery</h2>
                <p>The easy-living ambiance and lavish settings, coupled with our signature services ensure 
                    that stays at our hotel are excellent experiences, both for leisure and business travelers. 
                    We offer our guests five different accommodation options, that include immaculate rooms 
                    opening to views of the magnificent Taj Mahal.
                </p>
            </v-row>
              
          </section>   
        </v-content>
    </v-container>
      <v-col cols=12 md="12">
        <Carouselgallery/>
        <!-- Gallery carousel -->
      </v-col>
  </div>
</template>

<script>
</script>

<style>
.navbar {
  position: fixed;
  /* persistent throughout scrolling */
  top: 230px;
  /* position of v-sheet from top */
  z-index: 2;
  /* stacked on top of other elements */
  width: 10%;
  /* width of v-sheet */
  height: 120px;
  /* height of v-sheet */
  }
</style>
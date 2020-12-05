<template>
  <html>
    <div class="typeface">
    <!--class for poppins typeface  -->
      <v-row>
        <v-col cols="12" sm="12" md="12">
          <Breadcrumb/>
          <!-- Breadcrumb component -->
          <!-- section id ExploreAgra binds the section of the page to the Explore Agra link in the scrollspy--> 
          <Carouselmonuments/>
          <!-- Carousel component - monument pictures -->
          <!-- v-col defines number of columns, md defines size on medium screens -->
          <Navappear/>
          <!-- Nav bar for scrollspy appears for screen width less than lg -->
        </v-col>
        
        <v-col cols="12" md="12">
          <nav class="verticalnav">
            <Anchorbutton/>
            <!-- anchorbutton component is the vertical scrollspy visible in lg only -->
          </nav>
        </v-col>
      </v-row>
      
      <v-container class="mt-n16">
      <!-- container enables centering the site's componenents in a grid -->
        <v-content>
          <section id="ExploreAgra" >
          <!-- section id helps recognize section to bind to href links -->
            <v-col cols="12" sm="12" md="12">
              <v-row justify="center">
                <h1 class ="brandcol"> EXPLORE AGRA </h1>
                <!-- brandcol class for applying brand color to headings -->
              </v-row>  
              <!-- Explore Agra justified in the center, h1 for larger size of heading -->
                  <h2 class="font-size: 16pt; mt-4">Experience The Regal Charm of Agra, Uttar Pradesh</h2>   
                  <!-- h2 for a smaller size of heading in comparison with h1  -->
                    <p> 
                      We await to welcome you to the colourful vibes and regal charm of Agra. Experience the institutional hospitality of 
                      Crystal Sarovar Premiere — the perfect blend of luxury and convenience.As part of India's golden triangle, the city of Agra 
                      is one of the travel hotspots of the world. Agra, home to the Taj Mahal, one of the seven wonders of the world, is rich in its
                      history and architecture — chronicled landmarks, fantastic architecture marvels, altars, tombs devoted to love and celebration, 
                      forts, and palaces from the fabric of this city. But Agra has a lot more to offer. It is home to local artisians whose ancestors 
                      were makers of the Taj Mahal, there are bustling food streets and colorful flea markets like the Kinari bazar, birdwatching spots, and beautiful riversides.
                    </p>
                    <!-- paragraph tag -->
            </v-col>
          </section>
          
          <section id="Location">
          <!-- section id Location binds the section of the page to the Location link in the scrollspy-->
            <v-col cols="12" sm="12" md="12">
              <v-row justify="center">
                <h1 class ="brandcol">LOCATION</h1>
                  <Locationtabs/>
                  <!-- Tabs in location section -->
              </v-row>
          
              <v-row justify="left">
                <h2 class="font-size: 16pt; mt-8"> The Magnificent Taj Mahal </h2>
                <p class="font-size: 16pt; mt-4">
                  As part of India's golden triangle, the city of Agra is one of the travel hotspots of the world. 
                  Agra, home to the Taj Mahal, one of the seven wonders of the world, is rich in its history and 
                  archiecture. Taj Mahal, an epitome of love, is regarded as an astounding architectural beauty and 
                  has continuously been on the 'Seven Wonders of the World' list. Taj Mahal was constructed for a
                  period of 22 years, and a total of about twenty thousand workers were employed to build it. This 
                  architectural marvel is built entirely of white marble and it glows in the moonlight. Shah Jahan 
                  built this monument in the memory of his wife Mumtaz, whose grave is housed within the premises of 
                  the Taj Mahal. There are several other aspects that create the spectacle that the Taj Mahal is — beautiful 
                  Charbaghs(Taj Garden), the magnificent Darwaza,the symmetrical sandstone structures surrounding the Taj, 
                  and the placid Yamuna river that flows behind it.
                </p>
              </v-row>
            </v-col>
          </section>

          <section id="Dining">
          <!-- section id Dining binds the section of the page to the Dining link in the scrollspy-->
            <v-col cols="12" sm="12" md="12">
              <v-row justify="center">
                <h1 class ="brandcol"> DINING </h1>
                  <p class="align-center; mt-4"> 
                    We love to eat, to take our time and enjoy the flavours in a series of small dishes. Our degustation gives you the chance to do exactly that. 
                    More than a succession of plates, we offer you an experience, a connection between each dish, pulling from a wide range of authenticities.
                  </p>
                  <!-- aligning paragraph to the center -->
              </v-row>
            </v-col>
      

              <v-row justify="center">
              <!-- justify center for images -->
                <v-col cols="12" sm="6" md="5">
                  <v-img 
                  src="Cuisine meat 2.jpg" >

                  <template v-slot:placeholder>
                    <v-layout
                      fill-height
                      align-center
                      justify-center
                      ma-0
                    >
                      <v-progress-circular indeterminate color="#0A4082">
                      </v-progress-circular>
                    </v-layout>
                  </template>
                  <!-- Adding loaders -->
                  </v-img>
                  <!-- v-img to insert images sourced from static folder -->
                </v-col>
                  
              
                <v-col cols="12" sm="6" md="5">
                  <h2 class="font-size: 16pt; mt-4">ASSORTED BARBECUE CUISINE</h2>
                  <!-- h2 header size lower than h1 -->
                    <p class="mt-8">
                      Passion is the most important ingredient, and we bring you the 
                      beauty of barbecue flavours in every bite. Owing to our expert chefs, 
                      a nightly-changing tasting menu is sure to take your taste-buds on an 
                      adventurous ride into the beauty of the charcoal taste of barbecue food. 
                    </p>
                </v-col>
              </v-row>

              <v-row justify="center">
                <v-col cols="12" sm="6" md="5">
                  <v-img 
                  src="Cuisine French.jpg" >

                    <template v-slot:placeholder>
                      <v-layout
                        fill-height
                        align-center
                        justify-center
                        ma-0
                      >
                        <v-progress-circular indeterminate color="#0A4082">
                        </v-progress-circular>
                      </v-layout>
                    </template>
                    <!-- Adding loaders -->
                  </v-img>
                </v-col>

                <v-col cols="12" sm="6" md="5">
                <h2 class="font-size: 16pt; mt-4">ITALIAN CUISINE</h2>
                  <p class="mt-8">
                    Passion is the most important ingredient, and we bring you 
                    the beauty of Italian flavours in every bite. Owing to our expert chefs, 
                    a nightly-changing tasting menu is sure to take your taste-buds on an 
                    adventurous ride into the beauty of Italian food. 
                  </p>
                </v-col>
              </v-row>

              <v-row justify="center">
                <v-col cols="12" sm="6" md="5">
                  <v-img 
                  src="Cuisine Italian.jpg" >

                    <template v-slot:placeholder>
                      <v-layout
                        fill-height
                        align-center
                        justify-center
                        ma-0
                      >
                        <v-progress-circular indeterminate color="#0A4082">
                        </v-progress-circular>
                      </v-layout>
                    </template>
                    <!-- Adding loaders -->
                  </v-img>
                </v-col>

                <v-col cols="12" sm="6" md="5">
                  <h2 class="font-size: 16pt; mt-4">MEXICAN CUISINE</h2>
                  <p class="mt-8">Passion is the most important ingredient, and we bring you 
                    the beauty of Mexican flavours in every bite. Owing to our expert chefs, 
                    a nightly-changing tasting menu is sure to take your taste-buds on an 
                    adventurous ride into the beauty of Mexican food.</p>
                </v-col>
              </v-row>
          </section>   
                
          <section id="Gallery">
          <!-- section id Gallery binds the section of the page to the Gallery link in the scrollspy-->
            <v-row justify="center">
              <h1 class ="brandcol">GALLERY</h1>
                <p align="center">
                    The easy-living ambiance and lavish settings, coupled with our signature services ensure 
                    that stays at our hotel are excellent experiences, both for leisure and business travelers. 
                    We offer our guests five different accommodation options, that include immaculate rooms 
                    opening to views of the magnificent Taj Mahal.
                </p>
            </v-row>
          </section>   
          
        </v-content>
      </v-container>
        
      <v-row>
        <v-col cols=12 sm="12" md="12">
          <Carouselgallery/>
          <!-- Gallery carousel -->
        </v-col>
      </v-row>

        <p align="right" class="mr-16">
        <font size=2 color="#2699FB">
        <u>BOOK ROOMS</u>
        </font>
        </p>
    
    </div>
  </html>
</template>

<script>
</script>

<style>

  .verticalnav {
    position: fixed;
    /* persistent throughout scrolling */
    top: 230px;
    /* position of v-sheet from top */
    z-index: 2;
    /* stacked on top of other elements */
  }
  
  .typeface {
    font-family:"Poppins";} 
    
  @media (max-width: 600px){
  .subheadingsize{font-size: 16pt;}
  }
  /* subheading font size reduces for x */

  .brandcol {color:rgb(10, 64, 130);
  font-size: 28pt ;} 

  @media (max-width: 600px){
  .brandcol {
    font-size: 22pt;
  }
  }
  /* heading font size reduces in xs */

</style>


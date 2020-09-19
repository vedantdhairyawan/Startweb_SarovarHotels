<template>
  <div>
    <v-container>
        <v-content data-spy="scroll" data target="#navbar" data-offset="0">
          <nav>
            <ul>
              <li><a href="#Explore Agra">Explore Agra</a></li>
              <li><a href="#Location">Location</a></li>
              <li><a href="#Dining">Dining</a></li>
              <li><a href="#Gallery">Gallery</a></li>
            </ul>
          </nav>
      
            <v-col cols="12" sm="6" md="12">
              <Breadcrumb/>
              <Carouselhome/>
            </v-col>
          
              <section id="Explore Agra">
                <v-col cols="12" sm="6" md="12">
                  <v-row justify="center">
                    <h1> Explore Agra </h1>
                  </v-row>  
                      <h2>The Magnificent Taj Mahal</h2>      
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
                  </v-col>
              </section>

              <section id="Location">
                <v-col cols="12" sm="6" md="12">
                  <v-row justify="center">
                      <h1>Location</h1>
                  </v-row>
                </v-col>
                  <Growshrink/>
              </section>

              <section id="Dining">
                <v-col cols="12" sm="6" md="12">
                  <v-row justify="center">
                    <h1> Dining </h1>
                      <p align="center"> 
                        We love to eat, to take our time and enjoy the flavours in a series of small dishes. Our degustation gives you the chance to do exactly that. 
                        More than a succession of plates, we offer you an experience, a connection between each dish, pulling from a wide range of authenticities.
                      </p>
                  </v-row>
                </v-col>
        

                  <v-row justify="left">
                    <v-col cols="12" sm="6" md="5">
                      <v-img src="Cuisine meat 2.jpg" ></v-img>
                    </v-col>

                      <v-col cols="12" sm="6" md="7">
                        <h2>Assorted Barbecue Cuisine</h2>
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
                    <h2>French Cuisine</h2>
                      <p> Passion is the most important ingredient, and we bring you 
                          the beauty of Italian flavours in every bite. Owing to our expert chefs, 
                          a nightly-changing tasting menu is sure to take your taste-buds on an 
                          adventurous ride into the beauty of Italian food. </p>
                    </v-col>
                  </v-row>

                  <v-row justify="left">
                    <v-col cols="12" sm="6" md="5">
                      <v-img src="Cuisine Italian.jpg" ></v-img>
                    </v-col>

                    <v-col cols="12" sm="6" md="7">
                    <h2>Italian Cuisine</h2>
                    <p>Passion is the most important ingredient, and we bring you 
                      the beauty of Mexican flavours in every bite. Owing to our expert chefs, 
                      a nightly-changing tasting menu is sure to take your taste-buds on an 
                      adventurous ride into the beauty of Mexican food.</p>
                    </v-col>
                  </v-row>
              </section>   
                  
              <section id="Gallery">
                <v-row justify="center">
                  <h1>Gallery</h1>
                    <p>The easy-living ambiance and lavish settings, coupled with our signature services ensure 
                        that stays at our hotel are excellent experiences, both for leisure and business travelers. 
                        We offer our guests five different accommodation options, that include immaculate rooms 
                        opening to views of the magnificent Taj Mahal.
                    </p>
                </v-row>
                  <Carouselgallery/>
              </section>   
        </v-content>
    </v-container>
  </div>
</template>

<script>
</script>

<style>
</style>
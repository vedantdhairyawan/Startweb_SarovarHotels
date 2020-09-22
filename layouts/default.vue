<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="#FFFF" dark fixed app> 
      
      <!-- Component Example -->
      <Naviconinfo/>
      <Naviconsearch/>
      <SarovarLogo/>
      <Naviconprofile/>
    </v-app-bar>

    <!-- Body -->
    <v-content light>
      <nuxt /> 
    </v-content>
    
    <Footer/>
    <!-- <v-footer color="#000080" app>
      <span class="white--text">&copy; {{ new Date().getFullYear() }}</span>
    </v-footer> -->

  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .white--text {
    border: 1px solid;
  }

   #inspire {
    background-color: white;
    color: #707070 ;
  }
</style>
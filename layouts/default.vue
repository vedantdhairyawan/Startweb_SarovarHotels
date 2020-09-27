<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="#FFFF" dark fixed app> 
      
      <!-- Component Example -->
      <Naviconinfo/>
      <!-- information icon -->
      <Naviconmessage/>
      <!-- message icon -->
      <SarovarLogo/>
      <!-- hotel logo -->
      <Naviconprofile/>
      <!-- profile icon -->
    </v-app-bar>

      <!-- Body -->
    <v-content light>
      <nuxt /> 
    </v-content>
      
    <Footer/>
    
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
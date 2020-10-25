<template>
  <div>
    <v-breadcrumbs class="breadcrumbcolor" :items="items">
      <!-- applies breadcrumb class for color of text -->
      <template v-slot:divider>
      <!-- for introducing icons as dividers -->
        <v-icon color="grey darken-2">mdi-chevron-right</v-icon>
        <!-- breadcrumb arrow icons -->
      </template>
    </v-breadcrumbs>
  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Home',
          // visible breadcrumb text
          disabled: false,
          // boolean variable for being clickable (link disabled)
          
        },
        {
          text: 'Holidays',
          // visible breadcrumb text
          disabled: false,
          // boolean variable for being clickable (link disabled)
        },
        {
          text: 'Hotels',
          // visible breadcrumb text
          disabled: false,
          // boolean variable for being clickable (link disabled)
        },
        {
          text: 'Get details',
           // visible breadcrumb text
          disabled: false,
          // boolean variable for being clickable (link disabled)
        },
      ],
    }),
  }
</script>

<style>
.breadcrumbcolor {color:rgb(10, 64, 130);} 
/* sets the color for breadcrumb text */
</style>



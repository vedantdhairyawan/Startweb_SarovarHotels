<template>
  <div>
    <v-breadcrumbs :items="items">
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
          // boolean variable for being clickable
          href: 'Home',
          // href link
        },
        {
          text: 'Hotels',
          disabled: false,
          href: 'Hotels', 
        },
        {
          text: 'Crystal Sarovar Premiere,Agra',
          disabled: false,
          href: 'Crystal_Sarovar_Premiere_Agra',
        },
      ],
    }),
  }
</script>


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
          text: 'Holidays',
          // visible breadcrumb text
          disabled: false,
          // boolean variable for being clickable
          href: 'Holidays',
          // href link
        },
        {
          text: 'Hotels',
          disabled: false,
          href: 'Hotels', 
        },
        {
          text: 'Get details',
          disabled: false,
          href: 'Get details',
        },
      ],
    }),
  }
</script>


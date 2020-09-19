<template>
  <v-breadcrumbs :items="items">
    <template v-slot:item="{ item }">
      <v-breadcrumbs-item
        :href="item.href"
        :disabled="item.disabled"
      >
        {{ item.text.toUpperCase() }}
      </v-breadcrumbs-item>
    </template>
  </v-breadcrumbs>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Home',
          disabled: false,
          href: 'breadcrumbs_Home',
        },
        {
          text: 'Hotels',
          disabled: false,
          href: 'breadcrumbs_Hotels',
        },
        {
          text: 'Sarovar Portico, Agra',
          disabled: false,
          href: 'breadcrumbs_Sarovar_Portico,_Agra',
        },
      ],
    }),
  }
</script>
<template>
    <v-data-table
      :headers="headers"
      :items="desserts"
      :items-per-page="5"
      class="elevation-1"
    ></v-data-table>
  </template>
  
  <script>
  export default {
    data () {
      return {
        headers: [
          {
            text: 'Dessert (100g serving)',
            align: 'start',
            sortable: false,
            value: 'name',
          },
          { text: 'Student', value: 'Student' },
          { text: 'Lastname', value: 'Lastname' },
          { text: 'Firstname', value: 'Firstname' },
          { text: 'Middlename', value: 'Middlename' },
          { text: 'Course', value: 'Course' },
          {text: 'Section', value: 'Section' },

        ],
        desserts: [ ],
      }
    },
  }
</script>
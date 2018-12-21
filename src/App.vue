<script>
import LayoutDefault from './layouts/LayoutDefault'
import LayoutSimple from './layouts/LayoutSimple'

export default {
  computed: {
    layout () {
      return this.$store.getters.layout
    }
  },
  components: {
    'layout-default': LayoutDefault,
    'layout-simple': LayoutSimple
    // define as many layouts you want for the application
  }
}
</script>

<template>
  <v-app>
    <component v-bind:is="layout"></component>
  </v-app>
</template>

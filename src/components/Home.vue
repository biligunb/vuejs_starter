<script>
export default {
  methods: {
    setLayout (layout) {
      this.$store.commit('SET_LAYOUT', layout)
    }
  }
}
</script>

<template>
  <v-container fluid fill-height>
    <v-layout align-center justify-center>
      <v-btn color="primary" @click="setLayout('layout-simple')">Login Layout</v-btn>
      <v-btn color="secondary" @click="setLayout('layout-default')">Default Layout</v-btn>
    </v-layout>
  </v-container>
</template>

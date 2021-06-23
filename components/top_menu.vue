<template>
  <v-app-bar
      elevate-on-scroll
      color="grey lighten-5"
      dark
      app
      height="80px"
  >
    <v-container class="pa-0">
      <v-row no-gutters>
        <v-col
            cols="12"
            class="d-flex align-center"
        >
         <a href="#" class="indigo--text mr-auto">Logo</a>
         <a href="#services" class="indigo--text mr-4">Nossos serviços</a>
         <a href="#work" class="indigo--text">O que fazemos</a>

        </v-col>
      </v-row>
    </v-container>
  </v-app-bar>
</template>

<script>

export default {

}
</script>

<style lang="scss" scoped>
  a {
    text-decoration: none;
  }
</style>

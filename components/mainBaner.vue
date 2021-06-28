<template>
  <div class="white bg-main">
    <v-container py-16>
      <v-row style="height: 100vh">
        <v-col cols="12" sm="12" md="6"  lg="6" class="d-flex flex-column  align-center justify-center">
          <div class="text-center">
            <div class="indigo--text darken-4 text-h3 mb-4">
              TITULO
            </div>
            <div>
              Subtitulo
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>


<style lang="scss" scoped>
.bg-main {
  margin-top: -80px;
  background: url('/img/background-sherpa.png');
  text-align: center;
  background-size: cover;
  background-position: center;
  background-repeat:no-repeat;
}
</style>

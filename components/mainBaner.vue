<template>
  <div class="grey lighten-4 bg-main">
    <v-container py-16>
      <v-row style="height: 100vh">
        <v-col
          cols="12"
          sm="12"
          md="6"
          lg="6"
          class="d-flex flex-column justify-center align-center"
        >
          <div class="text-center mb-10">
            <div
              class="
                primary--text
                text-h3 text-md-h2 text-lg-h2
                font-weight-bold
                mb-4
              "
            >
              Você quer alcançar o topo?
            </div>
            <div class="text-subtitle-1 text-md-h6 text-lg-h6">
              O Marketing Digital exige dedicação, paciência e o desenvolvimento
              de novas habilidades.
            </div>
          </div>
          <v-btn color="primary" outlined x-large class="px-16 mt-10" href="#services"> Saiba mais </v-btn>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>


<style lang="scss" scoped>
.bg-main {
  margin-top: -80px;
  background: url("/sherpa/img/background-sherpa.png");
  text-align: center;
  background-size: cover;
  background-position: right;
  background-repeat: no-repeat;
}
</style>

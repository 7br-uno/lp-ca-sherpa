<template>
  <div class="bg-main">
    <v-container py-16>
      <v-row style="height: 100vh" class="mt-2">
        <v-col
          cols="12"
          sm="12"
          md="6"
          lg="6"
          class="d-flex flex-column justify-center align-lg-start align-center"
        >
            <div
              class="
                primary--text
                text-h3 text-md-h2 text-lg-h2
                font-weight-bold
                mb-4
                text-lg-left
                text-center
              "
            >
              Você quer <br> alcançar o topo?
            </div>
            <div class="text-h6 text-lg-left text-center ">
              O Marketing Digital exige dedicação, paciência e o desenvolvimento
              de novas habilidades.
            </div>
          <v-btn color="accent" x-large style="width: 300px" class="px-16 mt-10" href="#services"> Saiba mais </v-btn>
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
  background-color: #ebfbfe;
}
</style>

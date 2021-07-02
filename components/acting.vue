<template>
  <div class="grey lighten-3" id="acting">
    <v-container pt-16>
      <v-row>
        <v-col cols="12" class="text-h5 text-center text-uppercase mb-8 primary--text">
         Redes sociais vão alêm de postagens,<br />existem estratégias para que
        você se conecte com seu público.
        </v-col>
      </v-row>
      <v-row class="my-10">
        <v-col cols="12" sm="12" md="12" lg="6">
          <v-row>
            <v-col cols="12" class="d-flex justify-center text-h5 text-center">
              Atuamos de duas formas
            </v-col>
          </v-row>
          <v-row class="mb-8 px-6">
            <v-col cols="12" sm="6" md="6" lg="6">
              <v-card
                color="accent"
                class="
                  pa-4
                  d-flex
                  justify-center
                  text-center
                  white--text
                  card__atuacao
                "
              >
                Te ajudamos a se posicionar e definir objetivos
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="6">
              <v-card
                color="accent"
                class="
                  pa-4
                  d-flex
                  justify-center
                  text-center
                  white--text
                  card__atuacao
                "
              >
                Fazemos o serviço braçal pra sua jornada ficar mais leve
              </v-card>
            </v-col>
          </v-row>
        </v-col>
        <v-col  cols="12" sm="12" md="12" lg="6" class="d-flex justify-center align-center">
          <img src="/sherpa/img/estrategia.png" class="responsive_img" alt="">
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>
<style lang="scss" scoped>
.card__atuacao {
  display: flex;
  align-items: center;
}
.responsive_img {
  max-width: 80%;
  height: auto;
}
</style>

<template>
  <div class="grey lighten-3" id="acting">
    <v-container pt-16>
      <v-row>
        <v-col cols="12" class="d-flex flex-column align-center">
          <div class="text-h4 text-center text-uppercase primary--text mb-4">
            Redes sociais vão além de postagens!
          </div>
          <div class="text-h6 text-center">
            Existem estratégias para que você se conecte com seu público.
          </div>
        </v-col>
      </v-row>
      <v-row class="my-10" justify="center">
        <v-col cols="12" lg="6" class="d-flex justify-lg-end justify-center">
          <v-card class="d-flex align-center card__atuacao pa-10" rounded="xl">
            <img src="/sherpa/icons-2/target.png" style="width: 100px" class="mr-4"/>
            <div class="d-flex flex-column justify-center">
              <div class="text-body-1 primary--text font-weight-bold mb-2">Defina as metas</div>
              <div class="text-body-1 accent--text font-weight-medium">
                Vamos ajudar no seu posicionamento e a definir os objetivos!
              </div>
            </div>
          </v-card>
        </v-col>
        <v-col cols="12" lg="6" class="d-flex justify-lg-start justify-center">
          <v-card class="d-flex align-center card__atuacao pa-10" rounded="xl">
            <img src="/sherpa/icons-2/trekking.png" style="width: 100px" class="mr-4"/>
            <div class="d-flex flex-column justify-center">
              <div class="text-body-1 primary--text font-weight-bold mb-2">Mantenha o foco</div>
              <div class="text-body-1 accent--text font-weight-medium">
                Vamos fazer todo o serviço braçal para a sua jornada ficar mais leve!
              </div>
            </div>
          </v-card>
        </v-col>
      </v-row>
      <v-row class="mb-8">
        <v-col cols="12" class="d-flex justify-center">
          <v-btn
            color="accent"
            outlined
            x-large
            class="px-16 mt-10"
            href="#services"
            style="width: 300px"
          >
            Ver planos!
          </v-btn>
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
  height: 220px;
  max-width: 420px;
}
.responsive_img {
  max-width: 80%;
  height: auto;
}
</style>

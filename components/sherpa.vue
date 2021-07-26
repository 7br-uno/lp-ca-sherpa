<template>
  <div class="white" id="sherpa">
    <v-container py-16>
      <v-row>
        <v-col
          cols="12"
          class="
            primary--text
            text-uppercase text-h4 text-center
            mb-5
            d-flex
            justify-center
          "
        >
          <div>Nós seremos o <b>Sherpa</b> para o Corretor de Seguros</div>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          cols="12"
          sm="12"
          md="6"
          lg="6"
          class="d-flex align-center justify-center"
        >
          <img src="/sherpa/img/mochila.png" class="responsive_img" alt="" />
        </v-col>

        <v-col
          cols="12"
          sm="12"
          md="6"
          lg="6"
          class="d-flex flex-column text-justify align-center justify-center px-6"
        >
          <div class="body-1 mb-4">
            Após 3 anos oferecendo conteúdo de MKT Digital para Corretores de
            Seguros, entendemos que muitos precisam de um apoio maior.
          </div>
          <div class="body-1 mb-4">
            As redes sociais e tudo que as envolve, são uma bagagem extra para
            o Corretor de Seguros
          </div>
          <div class="body-1 mb-4">
            Quando se propõe a subir o Everest, os alpinistas treinam, se
            preparam, se equipam.
          </div>
          <div class="body-1 mb-4">Invariavelmente precisam de um Sherpa!</div>
          <v-btn color="primary" outlined x-large class="px-16 mt-10" href="#services" block> Saiba mais </v-btn>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="scss" scoped>
.responsive_img {
  max-width: 80%;
  height: auto;
}
</style>

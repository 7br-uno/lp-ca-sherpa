<template>
  <v-footer class="primary lighten-1 light-1 pt-6 pb-6 unselectable">
    <v-container class="pa-0">
      <v-row no-gutters>
        <v-col cols="12" class="d-flex align-center justify-center">
          <img src="/sherpa/img/logo-sherpa-1.png" class="logo" />
        </v-col>
        <!-- <v-col lg="6" md="6" sm="10" cols="7" class="d-flex align-center">
          <p class="w-100 mb-0 text-right text-md-center fs-10-pt white--text">
            <nobr>Siga nossas redes sociais:</nobr>
            <nobr>
              <v-btn
                class="ml-2"
                text
                icon
                color="accent"
                @click="go_to('https://instagram.com/clienteagente')"
              >
                <v-icon>mdi-instagram</v-icon>
              </v-btn>
              <v-btn
                class="ml-1"
                text
                icon
                color="accent"
                @click="
                  go_to('https://facebook.com/clienteagente')
                "
              >
                <v-icon>mdi-facebook</v-icon>
              </v-btn>
              <v-btn
                class="ml-1"
                text
                icon
                color="accent"
                @click="go_to('https://www.youtube.com/channel/UCscXKJvlhvWC4uvHXJ80oPg')"
              >
                <v-icon>mdi-youtube</v-icon>
              </v-btn>
              <v-btn
                class="ml-1"
                text
                icon
                color="accent"
                @click="go_to('https://www.linkedin.com/company/cliente-agente/')"
              >
                <v-icon>mdi-linkedin</v-icon>
              </v-btn>
            </nobr>
          </p>
        </v-col> -->
        <v-col
          cols="12"
          class="d-flex align-center justify-center"
        >
          <p class="mb-0 text-right fs-10-pt white--text">
            &copy; {{ new Date().getFullYear() }} Todos os direitos reservados.
          </p>
        </v-col>
        <v-col cols="12 mb-3 mb-md-0">
          <p class="mt-10 caption white--text text-center mb-16 mb-md-0">
            Criada em 2018 a Startup Cliente Agente foi pioneira na introdução
            do MKT de indicações para Corretores de Seguros no Brasil. Em 2019,
            lançamos o Studio Play, plataforma de MKT que permite obter
            conteúdos para as redes sociais e criação de Landing Pages. A
            Cliente Agente foi acelerada pela Oxigênio, Aceleradora de Startups
            da Porto Seguro e obteve investimento e mentoria da Plug´n Play, uma
            das maiores aceleradoras de Startups do Vale do Silício.
          </p>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  methods: {
    go_to(link) {
      window.open(link, "_blank");
    },
    go_home() {},
  },
};
</script>

<style>
.w-100 {
  width: 100%;
}
.fs-10-pt {
  font-size: 10pt;
}
.logo {
  /* height: 60px; */
  width: 300px;
  cursor: pointer;
}
</style>

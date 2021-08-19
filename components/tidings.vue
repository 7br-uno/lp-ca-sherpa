<template>
  <div class="accent py-8">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          class="text-center white--text text-h5 text-uppercase mb-2"
        >
          O que falam sobre nós:
        </v-col>
        <v-col cols="12">
          <v-card
            elevation="2"
            class="
              tidings
              grey
              lighten-5
              px-4
              d-flex
              align-center
              justify-center
              py-8
            "
          >
            <v-row justify="center">
              <v-col
                cols="12"
                md="6"
                lg="3"
                sm="6"
                v-for="(tiding, i) in tidings"
                :key="i"
              >
                <v-card class="mx-auto" max-width="260">
                  <v-img
                    class="white--text align-end"
                    height="200px"
                    :src="tiding.img"
                  >
                  </v-img>
                  <v-card-text class="text--primary">
                    <div>
                      <a
                        :href="tiding.link"
                        target="_blank"
                        rel="noopener noreferrer"
                        >{{tiding.title}}</a
                      >
                    </div>
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => {
    return {
      tidings: [
        {
          img: "https://i0.wp.com/jrs.digital/wp-content/uploads/2021/02/Kleber-de-Paula-Imagem-Divulgacao.jpg?resize=1024%2C813&ssl=1",
          link: "https://jrs.digital/2021/02/08/startup-cliente-agente-desenvolve-parceria-com-a-porto-seguro/",
          title:
            "Startup Cliente Agente desenvolve parceria com a Porto Seguro",
        },
        {
          img: "https://monitormercantil.com.br/wp-content/uploads/2020/11/Rede-sociais-696x617.jpg",
          link: "https://monitormercantil.com.br/cliente-agente-lanca-plataforma-de-videos-para-as-redes-sociais/",
          title:
            "Cliente Agente lança plataforma de vídeos para as redes sociais",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
a {
  text-decoration: none;
  &:hover {
    text-decoration: underline;
  }
}
</style>

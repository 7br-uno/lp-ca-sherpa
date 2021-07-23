<template>
  <div class="grey lighten-5" id="services">
    <v-container py-16>
      <v-row>
        <v-col cols="12" class="d-flex justify-center">
          <div class="primary--text text-h4 text-center text-uppercase mb-10">
            Conheça nossos pacotes de serviços
          </div>
        </v-col>
      </v-row>
      <v-row class="mb-6">
        <v-col
          cols="12"
          md="6"
          lg="3"
          sm="6"
          v-for="(service, i) in services"
          :key="i"
          class="d-flex justify-center"
        >
          <v-hover>
            <v-card class="service d-flex flex-column align-center pt-2">
              <span class="mb-2"></span>
              <!-- <div class="text-h6 text-uppercase font-weight-bold mb-2">
                {{ service.title }}
              </div> -->
              <!-- <div class="text-body-2 mb-2">
                {{ service.subtitle }}
              </div> -->
              <div
                :class="i % 2 == 0 ? 'primary' : 'accent'"
                class="
                  cicle
                  d-flex
                  align-center
                  justify-center
                  white--text
                  text-h6
                  font-weight-bold
                  my-4
                "
              >
                <div class="d-flex flex-column justify-center align-center">
                  <div class="text-h6 text-uppercase font-weight-bold mb-0">
                    {{ service.title }}
                  </div>
                  <span class="trace white"></span>
                </div>
              </div>

              <div class="pb-4 px-2">
                <ul v-if="i % 2 == 0">
                  <li
                    v-for="(listItem, i) in service.listItens"
                    :key="i"
                    class="pb-2"
                  >
                    <v-icon long color="primary"> mdi-check-circle </v-icon>
                    {{ listItem }}
                  </li>
                </ul>
                <ul v-else>
                  <li
                    v-for="(listItem, i) in service.listItens"
                    :key="i"
                    class="pb-2"
                  >
                    <v-icon long color="accent"> mdi-check-circle </v-icon>
                    {{ listItem }}
                  </li>
                </ul>
              </div>
              <v-btn
                class="white--text py-4 mb-8"
                :class="i % 2 == 0 ? 'primary' : 'accent'"
                @click="msg_whatsapp(service.msg)"
              >
                Solicite uma proposta
              </v-btn>
            </v-card>
          </v-hover>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-row class="mt-6">
        <v-col
          cols="12"
          md="6"
          lg="3"
          sm="6"
          v-for="(plane, i) in planes"
          :key="i"
        >
          <div class="text-h6">
            {{ plane.title }}
          </div>
          <div class="text-body-1 mb-2">
            {{ plane.subtitle }}
            <v-icon long color="grey">{{ plane.icon }}</v-icon>
          </div>
          <div class="text-body-2">
            {{ plane.description }}
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  methods: {
    msg_whatsapp(msg) {
      window.open(
        `https://api.whatsapp.com/send/?phone=55119402031620&text=${msg}`,
        "_blank"
      );
    },
  },
  data: () => {
    return {
      services: [
        {
          title: "Nepal",
          subtitle: "Para quem já tem Studio play",
          value: "299,00/mês",
          msg: "Quero conhecer o plano Nepal do projeto Sherpa",
          listItens: [
            "Setup das redes(Instagram e Facebook)",
            "Suporte com 8 postagens de conteúdos da Cliente Agente Studio",
            "Elaboração de 2 conteúdos personalizados/mês",
            "Orientação para produção de conteúdo autoral",
          ],
        },
        {
          title: "Base",
          msg: "Quero conhecer o plano Base do projeto Sherpa",
          subtitle: "Para quem já tem Studio play",
          value: "499,00/mês",
          listItens: [
            "Setup das redes(Instagram e Facebook)",
            "Suporte ao corretor com 12 postagens de conteúdos da Cliente Agente Studio",
            "Elaboração de 4 conteúdos personalizados/mês",
            "Orientação para produção de conteúdo autoral",
          ],
        },
        {
          title: "Himalaia",
          msg: "Quero conhecer o plano Himalaia do projeto Sherpa",
          subtitle: "Para quem já tem Studio play",
          value: "799,00/mês",
          listItens: [
            "Setup das redes(Instagram e Facebook)",
            "Suporte ao corretor com 16 postagens 12 da Cliente Agente Studio",
            "Elaboração de 4 conteúdos personalizados/mês",
            "2 anúncios (investimento em tráfego a parte)",
            "Orientação para conteúdo autoral",
          ],
        },
        {
          title: "Everest",
          msg: "Quero conhecer o plano Everest do projeto Sherpa",
          subtitle: "",
          value: "1399,00/mês",
          listItens: [
            "Orientação sobre posicionamento",
            "Setup das redes(Instagram e Facebook)",
            "Suporte com postagens diárias (Studio e personalizadas)",
            "4 anúncios (investimento em tráfego a parte)",
            "Orientação para produção de conteúdo autoral",
          ],
        },
      ],
      planes: [
        {
          title: "Nepal",
          subtitle: "Partida",
          icon: "mdi-contain-start",
          description:
            "Aqui, vamos planejar e seguir construindo a sua comunicação para conectar sua corretora com o público certo",
        },
        {
          title: "Base",
          subtitle: "Ambientação",
          icon: "mdi-desktop-mac-dashboard",
          description:
            "Estamos juntos na jornada, vamos nos preparar para começar a escalar",
        },
        {
          title: "Himalaia",
          subtitle: "Ritmo",
          icon: "mdi-run-fast",
          description:
            "Já na trajetória certa, vamos manter a frequência e criar autoridade",
        },
        {
          title: "Everest",
          subtitle: "Conquista",
          icon: "mdi-seal",
          description:
            "Consistência, coerência e constância em busca pelos objetivos traçados desde o inicio",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.service {
  width: 280px;
  flex-direction: column;
  justify-content: space-between;
}

.c-value {
  width: 100%;
}

ul {
  list-style: none;
}
.card__atuacao {
  display: flex;
  align-items: center;
}
.trace {
  width: 68px;
  height: 6px;
  border-radius: 4px;
  box-shadow: 1px 1px 1px 1px rgba(0, 0, 0, 0.2);
}
.cicle {
  height: 150px;
  width: 150px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
}
</style>

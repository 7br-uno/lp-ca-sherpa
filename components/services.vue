<template>
  <div class="grey lighten-5" id="services">
    <v-container pb-16 pt-8>
      <v-row>
        <v-col cols="12" class="d-flex justify-center pb-0">
          <div class="text-h5 text-center text-uppercase">
            Redes sociais vão alêm de postagens,
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12" class="d-flex justify-center pt-0">
          <div class="text-h5 text-center text-uppercase mb-10">
            existem estratégias para que você se conecte com seu público.
          </div>
        </v-col>
      </v-row>
      <v-row class="mb-10">
        <v-col cols="12" lg="4">
          <div class="card__atuacao d-flex justify-center text-h5">
            Atuamos de duas formas:
          </div>
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="4">
          <v-card
            color="indigo lighten-2"
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
        <v-col cols="12" sm="6" md="6" lg="4">
          <v-card
            color="indigo lighten-2"
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
      <v-row>
        <v-col cols="12" class="d-flex justify-center">
          <div class="indigo--text text-h4 text-center text-uppercase mb-10">
            Conheça nossos pacotes de serviços
          </div>
        </v-col>
      </v-row>
      <v-row>
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
            <v-card class="service d-flex flex-column align-center pt-8">
              <span class="trace grey lighten-1 mb-4"></span>
              <div class="text-h6 text-uppercase font-weight-bold mb-2">
                {{ service.title }}
              </div>
              <!-- <div class="text-body-2 mb-2">
                {{ service.subtitle }}
              </div> -->
              <div
                class="
                  indigo
                  lighten-2
                  cicle
                  d-flex
                  align-center
                  justify-center
                  white--text
                  text-h6
                  font-weight-bold
                  mb-4
                "
              >
                {{ service.value }}
              </div>

              <div class="pb-8 px-2">
                <ul>
                  <li
                    v-for="(listItem, i) in service.listItens"
                    :key="i"
                    class="pb-2"
                  >
                    <v-icon long color="indigo"> mdi-check-circle </v-icon>
                    {{ listItem }}
                  </li>
                </ul>
              </div>
              <v-btn class="indigo white--text py-4 mb-16">
                Aderir
              </v-btn>
            </v-card>
          </v-hover>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      services: [
        {
          title: "Nepal",
          subtitle: "Para quem já tem Studio play",
          value: "299,00/mês",
          listItens: [
            "Preparação das páginas",
            "Suporte com 8 postagens de conteúdos do Studio",
            "2 conteúdos personalizados/mês",
            "Orientação para conteúdo autoral",
          ],
        },
        {
          title: "Base",
          subtitle: "Para quem já tem Studio play",
          value: "499,00/mês",
          listItens: [
            "Preparação das páginas",
            "Suporte ao corretor com 12 postagens de conteúdos do Studio",
            "4 conteúdos personalizados/mês",
            "Orientação para conteúdo autoral",
          ],
        },
        {
          title: "Himalaia",
          subtitle: "Para quem já tem Studio play",
          value: "799,00/mês",
          listItens: [
            "Suporte ao corretor com 16 postagens 12 do cliente Agente Studio e 4 conteúdos personalizados",
            "2 anúncios (investimento em tráfego a parte)",
            "Orientação para conteúdo autora",
          ],
        },
        {
          title: "Everest",
          subtitle: "",
          value: "1399,00/mês",
          listItens: [
            "Preparação das páginas",
            "Post todo dia",
            "1 anuncio por semana (investimento em tráfego a parte)",
            "Orientação para conteúdo autora",
          ],
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

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

              <div class="pb-8 px-2">
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
              <v-btn class="white--text py-4 mb-16" :class="i % 2 == 0 ? 'primary' : 'accent'">
                Solicite prorposta
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

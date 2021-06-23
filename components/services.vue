<template>
  <div class="grey lighten-5">
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
          <v-card color="indigo lighten-2" class="pa-4 d-flex justify-center text-center white--text card__atuacao">
            Te ajudamos a se posicionar e definir objetivos
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="4">
          <v-card color="indigo lighten-2" class="pa-4 d-flex justify-center text-center white--text card__atuacao">
            Fazemos o serviço braçal pra sua jornada ficar mais leve
          </v-card>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12" class="d-flex justify-center">
          <div class=" indigo--text text-h4 text-center text-uppercase mb-10">
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
              <div class="text-h6 text-uppercase font-weight-bold">
                {{ service.title }}
              </div>
              <div class="text-body-2 mb-16">
                {{ service.subtitle }}
              </div>
              <div class="pb-8 px-2">
                <ul>
                  <li
                    v-for="(listItem, i) in service.listItens"
                    :key="i"
                    class="py-2"
                  >
                    <v-icon small color="indigo"> mdi-check-bold </v-icon>
                    {{ listItem }}
                  </li>
                </ul>
              </div>
              <div
                class="
                  c-value
                  indigo
                  white--text
                  d-flex
                  justify-center
                  align-center
                  font-weight-bold
                "
              >
                {{ service.value }}
              </div>
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
            "Orientação para conteúdo autora",
          ],
        },
        {
          title: "Nepal",
          subtitle: "Para quem já tem Studio play",
          value: "299,00/mês",
          listItens: [
            "Preparação das páginas",
            "Suporte com 8 postagens de conteúdos do Studio",
            "2 conteúdos personalizados/mês",
            "Orientação para conteúdo autora",
          ],
        },
        {
          title: "Nepal",
          subtitle: "Para quem já tem Studio play",
          value: "299,00/mês",
          listItens: [
            "Preparação das páginas",
            "Suporte com 8 postagens de conteúdos do Studio",
            "2 conteúdos personalizados/mês",
            "Orientação para conteúdo autora",
          ],
        },
        {
          title: "Nepal",
          subtitle: "Para quem já tem Studio play",
          value: "299,00/mês",
          listItens: [
            "Preparação das páginas",
            "Suporte com 8 postagens de conteúdos do Studio",
            "2 conteúdos personalizados/mês",
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
}

.c-value {
  width: 100%;
  height: 60px;
}

ul {
  list-style: none;
}
.card__atuacao {
  height: 80px;
  display: flex;
  align-items: center;
}
</style>

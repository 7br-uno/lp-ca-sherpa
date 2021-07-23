<template>
  <div class="bg-work" id="work">
    <v-container py-16>
      <v-row>
        <v-col cols="12">
          <div
            class="
              d-flex
              justify-center
              text-h5
              text-sm-h4 text-uppercase
              font-weight-bold
              text-center
              accent--text
            "
          >
            Evolua o nivel da sua marca
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          class="px-16 mt-8"
          lg="8"
          offset-lg="2"
        >
          <v-row>
            <v-col
              v-for="(work, i) in works"
              :key="i"
              cols="12"
              sm="6"
              md="4"
            >
              <v-hover>
                <template v-slot:default="{ hover }">
                  <div
                    :class="`elevation-${hover ? 16 : 4}`"
                    class="
                      mx-auto
                      transition-swing
                      card__work
                      rounded-circle
                      info
                      d-flex
                      flex-column
                      justify-center
                      align-center
                      text-center
                    "
                  >
                    <v-icon x-large color="white">
                      {{ work.icon }}
                    </v-icon>
                    <div class="text-body-1 mt-2 white--text">
                      {{ work.title }}
                    </div>
                  </div>
                </template>
              </v-hover>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => {
    return {
      works: [
        { title: "Sites", icon: "mdi-web" },
        {
          title: "Landing Pages personalizadas",
          icon: "mdi-page-layout-header",
        },
        { title: "Blog", icon: "mdi-book-open-page-variant" },
        {
          title: "Identidade Visual",
          icon: "mdi-account-supervisor-circle-outline",
        },
        { title: "Marca", icon: "mdi-head-lightbulb-outline" },
        { title: "Cartões Virtuais", icon: "mdi-card-account-details" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.card__work {
  height: 200px;
  text-align: center;
  width: 200px;
}

.bg-work {
  background-image: url('/sherpa/img/bolas.png');
  background-size: cover;
  background-position: center;
  background-repeat:no-repeat;
}
</style>

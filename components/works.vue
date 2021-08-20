<template>
  <div class="bg-work" id="work">
    <v-container py-16>
      <v-row>
        <v-col cols="12">
          <div
            class="
              d-flex
              justify-center
              text-sm-h4
              text-uppercase
              font-weight-bold
              text-center
              accent--text
              text-h6
            "
          >
            Evolua o nível da sua marca
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          class="px-16 mt-8"
          cols="12"
        >
          <v-row>
            <v-col
              v-for="(work, i) in works"
              :key="i"
              cols="12"
              sm="6"
              md="4"
              class="d-flex flex-column align-center"
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
                    <!-- <v-icon x-large color="white">
                      {{ work.icon }}
                    </v-icon> -->
                    <img :src="work.icon" style="width: 100px">
                  </div>
                </template>
              </v-hover>
                <div class="text-body-1 mt-2 primary--text font-weight-medium">
                  {{ work.title }}
                </div>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-row>
        <v-col offset="3" cols="6" class="d-flex justify-center">
          <v-btn color="primary" outlined x-large class="px-16 mt-10" href="#services" style="background: #ffffff; width: 300px"> Conheça as vantagens </v-btn>
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
        { title: "Sites", icon: "/sherpa/icons/computer (3).png" },
        {
          title: "Landing Pages",
          icon: "/sherpa/icons/landing-page.png",
        },
        { title: "Blog", icon: "/sherpa/icons/blog.png" },
        {
          title: "Identidade Visual",
          icon: "/sherpa/icons/swatches.png",
        },
        { title: "Marca", icon: "/sherpa/icons/branding.png" },
        { title: "Cartões Virtuais", icon: "/sherpa/icons/smartphone.png" },
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

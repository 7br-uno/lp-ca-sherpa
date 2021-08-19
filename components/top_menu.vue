<template>
  <v-app-bar
    elevate-on-scroll
    :color="windowTop === 0 ? 'transparent' : 'grey lighten-5'"
    dark
    app
    height="80px"
  >
    <v-container class="pa-0" fluid>
      <v-row no-gutters class="px-16">
        <v-col cols="12" class="d-flex align-center">
          <a href="#" class="mr-auto">
            <img
              v-if="windowTop === 0"
              src="/sherpa/img/logo-sherpa.png"
              class="logo-sherpa"
              alt="Sherpa"
            />
            <img
              v-if="windowTop > 0"
              src="/sherpa/img/logo-sherpa-1.png"
              class="logo-sherpa-1"
              alt="Sherpa"
            />
          </a>
          <div v-if="$vuetify.breakpoint.mdAndUp">
            <a href="#sherpa" class="accent--text mr-4">Quem somos</a>
            <a href="#acting" class="accent--text mr-4">Ações</a>
            <a href="#services" class="accent--text mr-4">Nossos serviços</a>
            <a href="#work" class="accent--text">O que fazemos</a>
          </div>
          <div class="d-flex d-md-none float-right">
            <v-menu
              transition="slide-y-transition"
              bottom
              min-width="94%"
              nudge-bottom="50"
            >
              <template v-slot:activator="{ on, attrs }">
                <v-btn
                  class="mx-2 mr-0"
                  fab
                  dark
                  small
                  color="accent"
                  v-bind="attrs"
                  v-on="on"
                >
                  <v-icon color="white"> mdi-menu </v-icon>
                </v-btn>
              </template>
              <v-list>
                <v-list-item-group color="accent">
                  <v-list-item to="#sherpa">
                    <v-list-item-title>Quem somos</v-list-item-title>
                  </v-list-item>
                  <v-list-item to="#acting">
                    <v-list-item-title>Ações</v-list-item-title>
                  </v-list-item>
                  <v-list-item to="#services">
                    <v-list-item-title>Nossos serviços</v-list-item-title>
                  </v-list-item>
                  <v-list-item to="#work">
                    <v-list-item-title>O que fazemos</v-list-item-title>
                  </v-list-item>
                </v-list-item-group>
              </v-list>
            </v-menu>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    go_to(link) {
      window.open(link, "_blank");
    },
  },

  data() {
    return {
      windowTop: 0,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.onScroll);
  },
  methods: {
    onScroll(e) {
      this.windowTop = e.target.documentElement.scrollTop;
    },
    go_to(link) {
      window.open(link, "_blank");
    },
  },
};
</script>

<style lang="scss" scoped>
a {
  text-decoration: none;
}
.logo-sherpa-1 {
  margin-top: 10px;
  height: 60px;
  cursor: pointer;
}

.logo-sherpa {
  margin-top: -30px;
  position: absolute;
  height: 150px;
  transition: height 0.2s;
  transition-timing-function: ease-in
}


.menu-links {
  color: white;
  text-decoration: none;
}
.fs-14 {
  font-size: 14px;
}
</style>

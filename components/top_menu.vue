<template>
  <v-app-bar
    elevate-on-scroll
    :color="windowTop === 0 ? 'transparent' : 'white'"
    dark
    app
    height="80px"
  >
    <v-container class="pa-0">
      <v-row no-gutters>
        <v-col
            cols="12"
            class="d-flex align-center"
        >
         <a href="#" class="indigo--text mr-auto">Logo</a>
         <a href="#acting" class="indigo--text mr-4">Ações</a>
         <a href="#services" class="indigo--text mr-4">Nossos serviços</a>
         <a href="#work" class="indigo--text">O que fazemos</a>
        </v-col>
      </v-row>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {
  data () {
    return {
      windowTop: 0
    }
  },
  mounted(){
    window.addEventListener("scroll", this.onScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.onScroll);
  },
  methods: {
    onScroll(e) {
      this.windowTop = e.target.documentElement.scrollTop;
    },
    go_to(link){
      window.open(link, "_blank");
    }
  }
}
</script>

<style lang="scss" scoped>
  a {
    text-decoration: none;
  }
</style>

<template>
  <v-app>
    <v-main class="pt-0 pb-0">
      <nuxt />
      <v-fab-transition v-if="float_wpp_btn">
        <v-btn @click="msg_whatsapp()" color="#00e676" dark fixed bottom right fab class="mb-5 mr-5">
          <v-icon>mdi-whatsapp</v-icon>
        </v-btn>
      </v-fab-transition>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data(){
    return{
      float_wpp_btn: false
    }
  },
  components: {
  },
  methods: {
    msg_whatsapp(){
      window.open('https://api.whatsapp.com/send/?phone=5511997343885&text=Quero saber como evoluir minha marca com projeto Sherpa', "_blank");
    }
  },
  mounted(){
    if($nuxt.$route.name !== 'telegram'){
      this.float_wpp_btn = true
    }
  },
  watch:{
    '$nuxt.$route.name'(){
      $nuxt.$route.name === 'telegram'
        ? this.float_wpp_btn = false
        : this.float_wpp_btn = true
    }
  }
}
</script>

<style>
*{scroll-behavior: smooth !important;}
</style>
